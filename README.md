check_drupal_messages
===========================

Hit a Drupal front page and check if are any status messages are displayed.

If none are found, the plugin returns status OK. The other two statuses are:
WARNING if it finds <div class="status warning"> and ERROR if it finds
<div class="status error">.

If you set error display to None via Configuration » Development » Logging and
errors, this plugin won't find any problems unless something really horrible
happened.

If you re-theme the status messages, you may need to pass the plugin different
text strings to look for using the -m option.

Usage: ./check_drupal_messages -U http://example.com/

---------------------------

Based on check_http_content-updated- by Vahid H.
  https://github.com/vahidhedayati/check_http_content-updated-
Based on check_http_content by CapSiDE SL.
  http://exchange.nagios.org/directory/Plugins/Websites%2C-Forms-and-Transactions/check_http_content/details

