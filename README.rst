
#################################
Daily Tarot - DivineAPI
#################################
Start your FREE Trial to get your API KEY,  `https://divineapi.com <https://divineapi.com>`_

|travis| |Docs| |Maintenance yes| |SayThanks| |Paypal|
    
    
.. image:: https://divineapi.com/assets/images/logo.svg
   :height: 412px
   :width: 898px
   :alt: divineapi logo
   :align: center
   
   

What is Daily Tarot API?
==============
Astrologers, Tarot Readers or Healers can now integrate astrology-related services to their website or application with Divine API. The data is related to all the important aspect of life that a person wants to know about. 

..
  Feel free to contribute on `Github <http://github.com/divineapi/horoscope-api>`_.




Why Daily Tarot API?
==========
Divine API puts an end to the search of any developer who is seeking for a Daily Tarot API which covers the aspects of life related to love life, career and money by picking a random card from a deck of 78 unique tarot card with images. 



Features
==========

- Daily Tarot API gives you a deck to choose cards from.
- It is a finely built API that tells you an accurate answer to your question.
- The chosen card reveals your personality,
- It also gives you advice in matters related to love finance and much more.
- You can pick as many cards as you want.


Benefits
==========

- With Daily Tarot API, you get a clear idea of your concerns.
- The user can think about a question and can seek near accurate answers and advice.
- Tarot reading acts as a relief providing tool.


URL
===
.. code-block:: python

    POST: https://divineapi.com/api/1.0/get_daily_tarot.php


Parameters
==========

api_key : 
   Your API  KEY.
   
   


Result Example:
=====
.. code-block:: json


      {
          "success": 1,
          "message": "Daily Tarot result.",
          "data": {
              "prediction": {
                  "card": "card1",
                  "category": "reverse",
                  "career": "C1",
                  "love": "L1",
                  "finance": "F1",
                  "image": "image_url"
              }
          }
      }


Example 
=======


cURL
^^^^
.. code-block:: curl

    curl -d "api_key=YOUR_API_KEY" -X POST https://divineapi.com/api/1.0/get_daily_tarot.php


Python
^^^^^^
.. code-block:: python

   import requests
   from requests.structures import CaseInsensitiveDict

   url = "https://divineapi.com/api/1.0/get_daily_tarot.php"

   headers = CaseInsensitiveDict()
   headers["Content-Type"] = "application/x-www-form-urlencoded"

   data = "api_key=YOUR_API_KEY"


   resp = requests.post(url, headers=headers, data=data)

   print(resp.status_code)


Javascript
^^^^^^^
.. code-block:: javascript

   var url = "https://divineapi.com/api/1.0/get_daily_tarot.php";

   var xhr = new XMLHttpRequest();
   xhr.open("POST", url);

   xhr.setRequestHeader("Content-Type", "application/x-www-form-urlencoded");

   xhr.onreadystatechange = function () {
      if (xhr.readyState === 4) {
         console.log(xhr.status);
         console.log(xhr.responseText);
      }};

   var data = "api_key=YOUR_API_KEY";

   xhr.send(data);


PHP
^^^
.. code-block:: php

   <?php
    $url = "https://divineapi.com/api/1.0/get_daily_tarot.php";

    $curl = curl_init($url);
    curl_setopt($curl, CURLOPT_URL, $url);
    curl_setopt($curl, CURLOPT_POST, true);
    curl_setopt($curl, CURLOPT_RETURNTRANSFER, true);

    $headers = array(
       "Content-Type: application/x-www-form-urlencoded",
    );
    curl_setopt($curl, CURLOPT_HTTPHEADER, $headers);

    $data = "api_key=YOUR_API_KEY";

    curl_setopt($curl, CURLOPT_POSTFIELDS, $data);

    $resp = curl_exec($curl);
    curl_close($curl);
    var_dump($resp);
   ?>
    
    
jQuery Ajax
^^^^^^
.. code-block:: javascript

    $.ajax({
   type:'POST',
   url:'https://divineapi.com/api/1.0/get_daily_tarot.php',
   data: {api_key:'YOUR_API_KEY'},
   success:function(data){
   console.log(data);
   }
    });


ECMAScript (ES6)
^^^^^^
.. code-block:: javascript

    const URL = 'https://divineapi.com/api/1.0/get_daily_tarot.php?api_key=YOUR_API_KEY';
    fetch(URL, {
        method: 'POST'
    })
    .then(response => response.json())
    .then(json => {
        const date = json.current_date;
        console.log(date);
    });


Services
========
|Horoscope| |Daily Tarot| |Yes No Tarot| |Fortune Cookie| |Coffee Cup|

License
=======

2021 Divine API

Licensed under the Apache License, Version 2.0 (the "License");

    http://www.apache.org/licenses/LICENSE-2.0



Contact
=======

Questions? Suggestions? Feel free to contact me at admin@divineapi.com


Credits
=======

"DivineAPI" was created by `Azhar <https://azhar-spiderdev.github.io/portfolio>`_

Source of updates - https://divineapi.com/daily-tarot-api

Please feel free to use and adapt this awesome API.

    

.. |Travis| image:: https://img.shields.io/badge/7%20Days%20Free%20trial-%23039BE5.svg?&style=for-the-badge&logoColor=white
    :target: https://divineapi.com/register

.. |SayThanks| image:: https://img.shields.io/badge/API%20Documentation-FCC624?style=for-the-badge&logoColor=white
    :target: https://divineapi.com/api-doc

.. |Paypal| image:: https://img.shields.io/badge/Other%20Services-%2311AB00.svg?&style=for-the-badge&logoColor=white
    :target: `Services`_
    
.. |Horoscope| image:: https://img.shields.io/badge/Daily%20Horoscope-cb22e6?style=for-the-badge&logoColor=white
    :target: https://github.com/divineapi/horoscope-api


.. |Daily Tarot| image:: https://img.shields.io/badge/Daily%20Tarot-cb22e6?style=for-the-badge&logoColor=white
    :target: https://github.com/divineapi/daily-tarot
    
    
.. |Yes No Tarot| image:: https://img.shields.io/badge/Yes%20Or%20No%20Tarot-cb22e6?style=for-the-badge&logoColor=white
    :target: https://github.com/divineapi/yes-or-no-tarot
    
.. |Fortune Cookie| image:: https://img.shields.io/badge/Fortune%20Cookie-cb22e6?style=for-the-badge&logoColor=white
    :target: https://github.com/divineapi/fortune-cookie
    
.. |Coffee Cup| image:: https://img.shields.io/badge/Coffee%20Cup-cb22e6?style=for-the-badge&logoColor=white
    :target: https://github.com/divineapi/coffee-cup-reading

.. Indices and tables
.. ==================

.. * :ref:`genindex`
.. * :ref:`modindex`
.. * :ref:`search`
