# [Plugin Handle]
# [User registration](https://github.com/annihilatoratm/joomla-doc/blob/main/doc-eng.md#user-registration)
# [Payment Flow](https://github.com/annihilatoratm/joomla-doc/blob/main/doc-eng.md#payment-flow-1)

  ## Plugin Handle
  ### Requirements
  * PHP 5.3 - 5.5
  * [curl extension](http://php.net/manual/en/book.curl.php)
  * [Joomla](http://www.joomla.org/download.html) 3.x (plugin v3.1)
  * [JoomShopping](http://joomshopping.pro/download/component.html) 4.x (plugin v4.3)
  

  ### Functionality
  - [x] [Sale Transactions](http://wiki.payneteasy.com/index.php/PnE:Sale_Transactions)
  - [ ] [Preauth/Capture Transactions](http://wiki.payneteasy.com/index.php/PnE:Preauth/Capture_Transactions)
  - [ ] [Transfer Transactions](http://wiki.payneteasy.com/index.php/PnE:Transfer_Transactions)
  - [ ] [Return Transactions](http://wiki.payneteasy.com/index.php/PnE:Return_Transactions)
  - [ ] [Recurrent Transactions](http://wiki.payneteasy.com/index.php/PnE:Recurrent_Transactions)
  - [x] [Payment Form Integration](http://wiki.payneteasy.com/index.php/PnE:Payment_Form_integration)
  - [ ] [Buy Now Button integration](http://wiki.payneteasy.com/index.php/PnE:Buy_Now_Button_integration)
  - [ ] [eCheck integration](http://wiki.payneteasy.com/index.php/PnE:eCheck_integration)
  - [ ] [Western Union Integration](http://wiki.payneteasy.com/index.php/PnE:Western_Union_Integration)
  - [ ] [Bitcoin Integration](http://wiki.payneteasy.com/index.php/PnE:Bitcoin_integration)
  - [ ] [Loan Integration](http://wiki.payneteasy.com/index.php/PnE:Loan_integration)
  - [ ] [Qiwi Integration](http://wiki.payneteasy.com/index.php/PnE:Qiwi_integration)
  - [ ] [Merchant Callbacks](http://wiki.payneteasy.com/index.php/PnE:Merchant_Callbacks)

  ### Package build
  1. [Composer installation](http://getcomposer.org/doc/00-intro.md), если его еще нет
  2. Clone the repo with plugin: `composer create-project payneteasy/php-plugin-joomshopping --stability=dev --prefer-dist`
  3. Go to plugin's directory: `cd php-plugin-joomshopping`
  4. compress the plugin directory into an archive: `composer archive --format=zip`

## <a name="get_package"></a> Получение пакета с плагином

  ### Installation
  1. [Get the plugin package](../README.md#get_package)
  2. Go to Joomla's admin panel
  3. Click on *Componenets* (1) -> *JoomShopping* (2) -> *Install & Update* (3).
  4. In the opened window click on *Choose File* (4) button and import the plugin package. Click on *Upload* (5) to upload it.
     
  <img src="/images/joomla-1-1-2.png" width=60% height=60%>

  ### Configuration
  1. Click on *Componenets* (1) -> *Options* (2) -> *Payments* (3).
  2. In the opened window two Payneteasy plugins can be configured: **Payneteasy sale form** (Form integration) and **PaynetEasy sale** (Direct integration).
  3. Click on the *Edit icon* (4) to start configuration.

  <img src="/images/joomla-1-1-2.png" width=60% height=60%>
  <img src="/images/joomla-1-1-3.png" width=60% height=60%>
  <img src="/images/joomla-1-1-4-form.png" width=60% height=60%>
  <img src="/images/joomla-1-1-4-direct.png" width=60% height=60%>

  ### Uninstallation

  # Удаление плагина

  1. In the **Payments** window select the methods that must be deleted.
  2. Click on *Delete* button at the top pf the page.

  <img src="/images/joomla-1-1-5.png" width=60% height=60%>
  
  3. For comlete uninstallation delete the following files from the Joomla's root directory
    * `components/vendor`
    * `components/com_jshopping/payments/pm_payneteasy_abstract`
    * `components/com_jshopping/payments/pm_payneteasy_sale`
    * `components/com_jshopping/payments/pm_payneteasy_saleform`


  ## User registration
  
  1. Click on *Create an account* to start the User registration process. Please fill all required parameters and press on *Register* button to finish registration.

  <img src="/images/joomla-register-1.png" width=60% height=60%>
  <img src="/images/joomla-register-2.png" width=60% height=60%>

  2. After registration performed you will be able to Log in into the Shop. 

  <img src="/images/joomla-register-3.png" width=60% height=60%>
  <img src="/images/joomla-register-4.png" width=60% height=60%>

  ## Payment Flow

  1. On the main page click on *Shop* to choose the category. Once category is chosed, select the needed item and press on *Buy* button. Press on *Checkout* button to continue.
  <img src="/images/joomla-1.png" width=60% height=60%>
  <img src="/images/joomla-2.png" width=60% height=60%>
  <img src="/images/joomla-3.png" width=60% height=60%>
  <img src="/images/joomla-4.png" width=60% height=60%>
  
  2. Fill all required parameters on Address and Delivery Method pages.

  <img src="/images/joomla-5.png" width=60% height=60%>
  <img src="/images/joomla-6.png" width=60% height=60%>

  3. On *Payment Method* page PaynetEasy sale method must be chosen. Please fill all mandatory fields.

  <img src="/images/joomla-7.png" width=60% height=60%>

  4. Confirm that you aware about **TERMS OF SERVICE and RETURN POLICY** and then *Confirm ordwer*. 

  <img src="/images/joomla-8.png" width=60% height=60%>
  <img src="/images/joomla-9.png" width=60% height=60%>
  <img src="/images/joomla-10.png" width=60% height=60%>
