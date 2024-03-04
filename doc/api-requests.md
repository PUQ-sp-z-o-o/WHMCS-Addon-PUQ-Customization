# API requests

#### To simply generate a promo code, use the link generated when creating a set to get the required promo code by invoking the cURL command:

- Clicking on the set name or ID opens a template for editing a Promo Set.

[![edit promo set.png](https://doc.puq.info/uploads/images/gallery/2024-01/scaled-1680-/edit-promo-set.png)](https://doc.puq.info/uploads/images/gallery/2024-01/edit-promo-set.png)

- Copy an URL next to IP Adress"

#### [![promo url 3.png](https://doc.puq.info/uploads/images/gallery/2024-01/scaled-1680-/promo-url-3.png)](https://doc.puq.info/uploads/images/gallery/2024-01/promo-url-3.png)

**Method**: POST

**Example:**

```
curl \
-X POST YOUR_URL_FROM_SET
```

**Response example:**

```
{
    "id": 61,
    "code": "XABKKA",
    "type": "Percentage",
    "recurring": 1,
    "value": "25.50",
    "cycles": "Quarterly,Semi-Annually,Annually,5Years,6Years,7Years",
    "appliesto": "12,40,18",
    "requires": "13,50,D.ua",
    "requiresexisting": 0,
    "startdate": "2024-01-01",
    "expirationdate": "2024-01-27",
    "maxuses": 11,
    "uses": 0,
    "lifetimepromo": 0,
    "applyonce": 1,
    "newsignups": 1,
    "existingclient": 0,
    "onceperclient": 0,
    "recurfor": 0,
    "upgrades": 1,
    "upgradeconfig": "a:4:{s:5:\"value\";s:2:\"11\";s:4:\"type\";s:7:\"product\";s:12:\"discounttype\";s:10:\"Percentage\";s:13:\"configoptions\";a:2:{i:0;s:2:\"11\";i:1;s:2:\"13\";}}",
    "notes": "TEST TEST"
}
```

####  

#### You can also include some additional data if needed:

`name` - Adds the beginning of the promo code for clarity regarding its set association.

`value` - Specifies the value for promo codes.

`promo_code_type` - Specifies the discount type for promo codes, which can be:

- Percentage
- Fixed Amount
- Price Override
- Free Setup

`start_date` - Specifies the promo code's access start date.

`expiry_date` - Specifies the promo code's access end date.

`notes` - Adds notes from the author.

**Method**: POST

**Example:**

```
curl \
-X POST YOUR_URL_FROM_SET \
-d "name=puqcloud.com&\
value=50&\
promo_code_type=Fixed Amount&\
start_date=2024-01-01&\
expiry_date=2024-12-30&\
notes=TEST FOR DOCUMENTATION"
```

**Response example:**

```
{
    "id": 66,
    "code": "puqcloud.com-PFC",
    "type": "Fixed Amount",
    "recurring": 1,
    "value": "50.00",
    "cycles": "Quarterly,Semi-Annually,Annually,5Years,6Years,7Years",
    "appliesto": "12,40,18",
    "requires": "13,50,D.ua",
    "requiresexisting": 0,
    "startdate": "2024-01-01",
    "expirationdate": "2024-12-30",
    "maxuses": 11,
    "uses": 0,
    "lifetimepromo": 0,
    "applyonce": 1,
    "newsignups": 1,
    "existingclient": 0,
    "onceperclient": 0,
    "recurfor": 0,
    "upgrades": 1,
    "upgradeconfig": "a:4:{s:5:\"value\";s:2:\"11\";s:4:\"type\";s:7:\"product\";s:12:\"discounttype\";s:10:\"Percentage\";s:13:\"configoptions\";a:2:{i:0;s:2:\"11\";i:1;s:2:\"13\";}}",
    "notes": "TEST FOR DOCUMENTATION"
}
```

**Errors:**

```
- The expiry date must be a date in the future.
- The expiry date must be later than the start date.
```

#### If you send a request using the GET method, it will return information about the network:

**Method**: GET

**Example:**

```
curl \
-X GET YOUR_URL_FROM_SET
```

**Response example:**

```
{
    "id": 1,
    "name": "test",
    "api_ip_address": "77.87.125.4",
    "api_key": "XJCRRFKY9GZ55CDR9H98NFJND",
    "promo_code_type": "Percentage",
    "recurring": 1,
    "recur_for": 0,
    "promo_value": 25.5,
    "applies_to": [
        "12",
        "40",
        "18"
    ],
    "requires": [
        "13",
        "50",
        "D.ua"
    ],
    "requires_existing": 0,
    "cycles": [
        "Quarterly",
        "Semi-Annually",
        "Annually",
        "5Years",
        "6Years",
        "7Years"
    ],
    "start_date": "2024-01-01",
    "expiration_date": "2024-01-27",
    "max_uses": 11,
    "lifetime_promo": 0,
    "apply_once": 1,
    "new_signups": 1,
    "once_per_client": 0,
    "existing_client": 0,
    "upgrades": 1,
    "upgrade_type": "product",
    "upgrade_discount_type": "Percentage",
    "upgrade_value": "11",
    "config_option_upgrades": [
        "11",
        "13"
    ],
    "notes": "TEST TEST",
    "url": "XJCRRFKY9GZ55CDR9H98NFJND-1-7dc8108e1a78c37c136732d464208a22"
}
```

<div id="bkmrk--1"></div>