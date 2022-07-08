# WooCommerce

## Файлы шаблонов

- [Основные](#основные)
- [Корзина](#корзина)
- [Оформление заказа](#оформление-заказа)
- [Почтовые сообщения](#почтовые-сообщения)
- [Общие](#общие)
- [Циклы](#циклы)
- [Личный кабинет](#личный-кабинет)
- [Уведомления](#уведомления)
- [Заказ](#заказ)
- [Карточка товара](#карточка-товара)

### Основные

<details>
  <summary>Click</summary>
  <p>1. <b>archive-product.php</b> - шаблон главного цикла вывода товаров</p> 
  <p>2. <b>content-product.php</b> - шаблон вывода товара, woocommerce_content()</p> 
  <p>3. <b>content-product_cat.php</b> - шаблон вывода товара в категории, шорткод [product_categories]. woocommerce_product_subcategories()</p> 
  <p>4. <b>content-single-product.php</b> - шаблон вывода одиночного товара, woocommerce_content()</p>
  <p>5. <b>content-widget-product.php</b> - шаблон вывода товара в стандартных виджетах</p> 
  <p>6. <b>product-searchform.php</b> - шаблон формы поиска товаров, get_product_search_form()</p> 
  <p>7. <b>single-product.php основной</b> - шаблон карточки товара</p>
  <p>8. <b>single-product-reviews.php</b> - шаблон вывода комментариев</p>  
  <p>9. <b>taxonomy-product_cat.php</b> - шаблон выводит товары категории, вызывает archive-product.php</p> 
  <p>10. <b>taxonomy-product_tag.php</b> - шаблон выводит товары метки, вызывает archive-product.php</p>
</details>

### Корзина

<details>
  <summary>Click</summary>
  <p>11. <b>cart\cart.php</b> - шаблон вывода корзины с помощью шорткода, WC_Shortcode_Cart::Output()</p>
  <p>12. <b>cart\cart-empty.php</b> - шаблон вывода пустой корзины с помощью шорткода, WC_Shortcode_Cart::Output()</p>
  <p>13. <b>cart\cart-item-data.php</b> - шаблон элементов данных + вариаций в корзине, WC_Cart::get_item_data()</p>
  <p>14. <b>cart\cart-shipping.php</b> - шаблон получения методов доставки в корзине, wc_cart_totals_shipping_html()</p>
  <p>16. <b>cart\cart-totals.php</b> - шаблон итоговых сумм, woocommerce_cart_totals()</p>
  <p>17. <b>cart\cross-sells.php</b> - шаблон перекрестных продаж, woocommerce_cross_sell_display()</p>
  <p>18. <b>cart\mini-cart.php</b> - шаблон вывода мини-корзины в виджете, woocommerce_mini_cart()</p>
  <p>19. <b>cart\shipping-calculator.php</b> - шаблон калькулятора доставки, woocommerce_shipping_calculator()</p>
</details>

### Оформление заказа

<details>
  <summary>Click</summary>
  <p>20. <b>checkout\cart-errors.php</b> - шаблон ошибок при оформлении заказа, WC_Shortcode_Checkout::checkout() </p>
  <p>21. <b>checkout\form-billing.php</b> - шаблон формы платежной информации, WC_Shortcode_Checkout::checkout()</p>
  <p>22. <b>checkout\form-checkout.php</b> - шаблон формы оформления заказа , WC_Shortcode_Checkout::checkout()</p>
  <p>23. <b>checkout\form-coupon.php</b> - шаблон формы купона, woocommerce_checkout_coupon_form()</p>
  <p>24. <b>checkout\form-login.php</b> - шаблон формы логина при оформлении заказа, woocommerce_checkout_login_form()</p>
  <p>25. <b>checkout\form-pay.php</b> - шаблон формы оплаты, WC_Shortcode_Checkout::Order_pay()</p>
  <p>26. <b>checkout\form-shipping.php</b> - шаблон формы доставки, WC_Checkout::checkout_form_shipping()</p>
  <p>27. <b>checkout\payment.php</b> - шаблон оплаты при оформлении заказа, woocommerce_checkout_payment</p>
  <p>28. <b>checkout\payment-method.php</b> - шаблон вывода метода оплаты, из шаблона checkout\payment.php</p>
  <p>29. <b>checkout\review-order.php</b> - шаблон таблицы заказа, woocommerce_order_review()</p>
  <p>30. <b>checkout\thankyou.php</b> - шаблон вывода сообщений при оформлении заказа, WC_Shortcode_Checkout::Order_received()</p>
</details>

### Почтовые сообщения

<details>
  <summary>Click</summary>
  <p>31. <b>emails\plain\admin-cancelled-order.php</b> - шаблон электронного письма админу об отмененном заказе в текстовом формате, класс WC_Email_Cancelled_Order</p>
  <p>32. <b>emails\plain\admin-new-order.php</b> - шаблон электронного письма админу о новом заказе в текстовом формате, класс WC_Email_New_Order</p>
  <p>33. <b>emails\plain\customer-completed-order.php</b> - шаблон электронного письма о завершении отправляются клиентам во время пометки заказов как выполненные и обычно отражают факт успешной доставки в текстовом формате, класс WC_Email_Customer_Completed_Order</p>
  <p>34. <b>emails\plain\customer-invoice.php</b> - шаблон электронного письма со счетом на оплату отправляются клиентам и содержат информацию о заказе и ссылки для оплаты в текстовом формате, класс WC_Email_Customer_Invoice</p>
  <p>35. <b>emails\plain\customer-new-account.php</b> - шаблон электронного письма о создании учетной записи отправляются клиенту после создания учетной записи на страницах оплаты или учетной записи в текстовом формате, класс WC_Email_Customer_New_Account</p>
  <p>36. <b>emails\plain\customer-note.php</b> - шаблон электронного письма с заметкой отправляется клиенту, когда вы добавляете заметку к заказу в текстовом формате, класс WC_Email_Customer_Note</p>
  <p>37. <b>emails\plain\customer-processing-order.php</b> - шаблон электронного письма уведомление содержит детали заказа и отправляется клиенту после оплаты в текстовом формате, класс WC_Email_Customer_Processing_Order</p>
  <p>38. <b>emails\plain\customer-reset-password.php</b> - шаблон электронного письма «сброса пароля» отправляются, когда пользователи сбрасывают свои пароли, класс WC_Email_Customer_Reset_Password</p>
  <p>39. <b>emails\plain\email-addresses.php</b> - шаблон для формирования электронного адреса в текстовом формате, WC_Emails::email_addresses</p>
  <p>40. <b>emails\plain\email-order-items.php</b> - шаблон для формирования элементов заказа (SKU, Заголовок, Стоимость и т.д.) в текстовом формате, WC_Abstract_Order::email_order_items_table</p>
  <p>41. <b>emails\admin-cancelled-order.php</b> - шаблон для html-формата, см. emails\plain\admin-cancelled-order.php</p>
  <p>42. <b>emails\admin-new-order.php</b> - шаблон для html-формата, см. emails\plain\admin-new-order.php</p>
  <p>43. <b>emails\customer-completed-order.php</b> - шаблон для html-формата, см. emails\plain\customer-completed-order.php</p>
  <p>44. <b>emails\customer-invoice.php</b> - шаблон для html-формата, см. emails\plain\customer-invoice.php</p>
  <p>45. <b>emails\customer-new-account.php</b> - шаблон для html-формата, см. emails\plain\customer-new-account.php</p>
  <p>46. <b>emails\customer-note.php</b> - шаблон для html-формата, см. emails\plain\customer-note.php</p>
  <p>47. <b>emails\customer-processing-order.php</b> - шаблон для html-формата, см. emails\plain\customer-processing-order.php</p>
  <p>48. <b>emails\customer-reset-password.php</b> - шаблон для html-формата, см. emails\plain\customer-reset-password.php</p>
  <p>49. <b>emails\email-addresses.php</b> - шаблон для html-формата, см. emails\plain\email-addresses.php</p>
  <p>50. <b>emails\email-footer.php</b> - шаблон для «подвала» электронного письма</p>
  <p>51. <b>emails\email-header.php</b> - шаблон для «шапки» электронного письма</p>
  <p>52. <b>emails\email-order-items.php</b> - шаблон для html-формата, см. emails\plain\email-order-items.php</p>
  <p>53. <b>emails\email-styles.php</b> - шаблон для стилевого оформления электронного письма</p>
</details>

### Общие

<details>
  <summary>Click</summary>
  <p>54. <b>global\breadcrumb.php</b> - шаблон вывода «хлебных крошек», woocommerce_breadcrumb()</p>
  <p>55. <b>global\form-login.php</b> - шаблон формы логина, woocommerce_login_form()</p>
  <p>56. <b>global\quantity-input.php</b> - шаблон поля количества для добавления в корзину, woocommerce_quantity_input()</p>
  <p>57. <b>global\sidebar.php</b> - шаблон вывода сайдбара, woocommerce_get_sidebar()</p>
  <p>58. <b>global\wrapper-end.php</b> - шаблон окончания врапера страницы, woocommerce_output_content_wrapper_end()</p>
  <p>59. <b>global\wrapper-start.php</b> - шаблон начала врапера страницы, woocommerce_output_content_wrapper()</p>
</details>

### Циклы

<details>
  <summary>Click</summary>
  <p>60. <b>loop\add-to-cart.php</b> - шаблон добавление в корзину для цикла товаров, woocommerce_template_loop_add_to_cart()</p>
  <p>61. <b>loop\loop-end.php</b> - шаблон окончания цикла вывода товаров, woocommerce_product_loop_end()</p>
  <p>62. <b>loop\loop-start.php</b> - шаблон начала цикла вывода товаров, woocommerce_product_loop_start()</p>
  <p>63. <b>loop\no-products-found.php</b> - шаблон вывода информации о не найденных товарах, woocommerce_content()</p>
  <p>64. <b>loop\orderby.php</b> - шаблон вывода списка сортировок в цикле, woocommerce_catalog_ordering()</p>
  <p>65. <b>loop\pagination.php</b> - шаблон пагинации в цикле, woocommerce_pagination()</p>
  <p>66. <b>loop\price.php</b> - шаблон цены товара в цикле товаров, woocommerce_template_loop_price()</p>
  <p>67. <b>loop\rating.php</b> - шаблон вывода суммарного рейтинга в цикле товаров, woocommerce_template_loop_rating()</p>
  <p>68. <b>loop\result-count.php</b> - шаблон вывода найденного количество в цикле в виде «Показано 5 из 10», woocommerce_result_count()</p>
  <p>69. <b>loop\sale-flash.php</b> - шаблон продаж в цикле товаров, woocommerce_show_product_loop_sale_flash()</p>
</details>

### Личный кабинет

<details>
  <summary>Click</summary>
  <p>70. <b>myaccount\form-add-payment-method.php</b> - шаблон добавления метода оплаты</p>
  <p>71. <b>myaccount\form-edit-account.php</b> - шаблон формы редактирования своего аккаунта</p>
  <p>72. <b>myaccount\form-edit-address.php</b> - шаблон формы редактирования адреса</p>
  <p>73. <b>myaccount\form-login.php</b> - шаблон формы входа в личный кабинет</p>
  <p>74. <b>myaccount\form-lost-password.php</b> - шаблон формы отправки пароля на электронную почту</p>
  <p>75. <b>myaccount\my-account.php</b> - шаблон вывода личного кабинета</p>
  <p>76. <b>myaccount\my-address.php</b> - шаблон вывода адреса</p>
  <p>77. <b>myaccount\my-downloads.php</b> - шаблон вывода загружаемых товаров</p>
  <p>78. <b>myaccount\my-orders.php</b> - шаблон вывода заказов</p>
  <p>79. <b>myaccount\view-order.php</b> - шаблон просмотра заказа</p>
</details>

### Уведомления

<details>
  <summary>Click</summary>
  <p>80. <b>notices\error.php</b> - шаблон вывода сообщений об ошибках</p>
  <p>81. <b>notices\notice.php</b> - шаблон вывода предупреждений</p>
  <p>82. <b>notices\success.php</b> - шаблон вывода сообщений об успешных действиях</p>
</details>

### Заказ

<details>
  <summary>Click</summary>
  <p>83. <b>order\form-tracking.php</b> - шаблон вывода отслеживания заказа, шорткод [woocommerce_order_tracking]</p>
  <p>84. <b>order\order-again.php</b> - шаблон кнопки «Повторить заказ», woocommerce_order_again_button()</p>
  <p>85. <b>order\order-details.php</b> - шаблон таблицы заказа, woocommerce_order_details_table()</p>
  <p>86. <b>order\tracking.php</b> - шаблон вывода отслеживания заказа, шорткод [woocommerce_order_tracking]</p>
</details>

### Карточка товара

<details>
  <summary>Click</summary>
  <p>87. <b>single-product\add-to-cart\external.php</b> - шаблон вывода области добавления в корзину для внешнего товара , woocommerce_external_add_to_cart()</p>
  <p>88. <b>single-product\add-to-cart\grouped.php</b> - шаблон вывода области добавления в корзину для группового товара , woocommerce_grouped_add_to_cart()</p>
  <p>89. <b>single-product\add-to-cart\simple.php</b> - шаблон вывода области добавления в корзину для простого товара, woocommerce_simple_add_to_cart()</p>
  <p>90. <b>single-product\add-to-cart\variable.php</b> - шаблон вывода области добавления в корзину для вариативного товара , woocommerce_variable_add_to_cart()</p>
  <p>91. <b>single-product\tabs\additional-information.php</b> - шаблон вывода содержимого вкладки «Информация», woocommerce_product_additional_information_tab()</p>
  <p>92. <b>single-product\tabs\description.php</b> - шаблон вывода содержимого вкладки «Описание», woocommerce_product_description_tab()</p>
  <p>93. <b>single-product\tabs\tabs.php</b> - шаблон вывода вкладок в карточке товара, woocommerce_output_product_data_tabs()</p>
  <p>94. <b>single-product\meta.php</b> - шаблон вывода артикула, категорий, меток товара в карточке товара, woocommerce_template_single_meta()</p>
  <p>95. <b>single-product\price.php</b> - шаблон вывода цены в карточке товара, woocommerce_template_single_price()</p>
  <p>96. <b>single-product\product-attributes.php</b> - шаблон вывода атрибутов товара, WC_Product::list_attributes()</p>
  <p>97. <b>single-product\product-image.php</b> - шаблон основной картинки в карточке товара, woocommerce_show_product_images()</p>
  <p>98. <b>single-product\product-thumbnails.php</b> - шаблон миниатюр в карточке товаров, woocommerce_show_product_thumbnails()</p>
  <p>99. <b>single-product\rating.php</b> - шаблон вывода рейтинга товара в карточке товара, woocommerce_template_single_rating()</p>
  <p>100. <b>single-product\related.php</b> - шаблон вывода сопутствующих товаров, woocommerce_related_products()</p>
  <p>101. <b>single-product\review.php</b> - шаблон вывода комментариев, woocommerce_comments()</p>
  <p>102. <b>single-product\sale-flash.php</b> - шаблон вывода метки «Распродажа» в карточке товара, woocommerce_show_product_sale_flash()</p>
  <p>103. <b>single-product\share.php</b> - шаблон вывода продукта обмена в карточке товара, woocommerce_template_single_sharing()</p>
  <p>104. <b>single-product\short-description.php</b> - шаблон вывода краткого описания в карточке товара, woocommerce_template_single_excerpt()</p>
  <p>105. <b>single-product\title.php</b> - шаблон вывода заголовка товара в карточке товара, woocommerce_template_single_title()</p>
  <p>106. <b>single-product\up-sells.php</b> - шаблон вывода рекомендованных товаров, woocommerce_upsell_display()</p>
</details>
