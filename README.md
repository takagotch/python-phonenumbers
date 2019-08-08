### python-phonenumbers
---
https://github.com/daviddrysdale/python-phonenumbers

```py
import phonenumbers
x = phonenumbers.parse("", None)
print(x)
type(x)
y = phonenumbers.parse("", "GB")
y = phonenumbers.parse("020 8366 1177", "GB")
print(y)
x == y
z = phonenumbers.parse("00 1 650 253 2222", "GB")
print(z)

z = phonenumbers.parse("", None)
print(z)
phonenumbers.is_valid_number(z)
z = phonnumbers.parse("", None)
print(z)
phonenumbers.is_possible_number(z)
phonenumbers.is_valid_number(z)

z = phonenumbers.parse("", None)
z = phonenumbers.parse("", None)

phonenumbers.format_number(x, PhoneNumberFormat.NATIONAL)
phonenumbers.format_number()
phonenumbers.format_number()

formatter = phonenumbers.AsYouTypeFormatter("US")
formatter.input_digit("6")
formatter.input_digit("5")
formatter.input_digit("0")
formatter.input_digit("2")
formatter.input_digit("5")
formatter.input_digit("3")
formatter.input_digit("2")
formatter.input_digit("2")
formatter.input_digit("2")
formatter.input_digit("2")
formatter.input_digit("2")

text = "Call me at 510-748-8230 if it's before 9:30, or 703-4800500 after 10am."
for match in phonenumbers.PhoneNumberMatcher(text, "US"):
  print(match)
for match in phonenumbers.PhoneNumberMatcher(text, "US"):
  print(phonenumbers.format_number(match.number, phonenumbers.PhoneNumberFormat.E164))

from phonenumbers import geocoder
ch_number = phonenumbers.parse("043123467", "CH")
geocoder.description_for_number(ch_number, "de")
geocoder.description_for_number(ch_number, "en")
geocoder.description_for_number(ch_number, "fr")
geocoder.description_for_number(ch_number, "it")

from phonenumbers import carrier
ro_number = phonenumbers.parse("+40721234567", "RO")
carrier.name_for_number(ro_numbre, "en")

from phonenumbers import timezone
gb_number = phonenumbers.parse("+447986123456", "GB")
timezone.time_zones_for_number(gb_number  )
```

```sh
pip install phonenumbers
```

```
```


