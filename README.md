<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

# xxAI.art दा

वेबसाइट कोड दा इक हिस्सा ओपन सोर्स ऐ, अनुवाद गी अनुकूल बनाने च मदद करने लेई तुंदा सुआगत ऐ।

## फ्रंट-एंड कोड

* [फ्रंट-एंड कोड](https://github.com/xxai-art/web)
* [समग्र रूप कन्नै साइट आस्तै भाशा पैक](https://github.com/xxai-art/web/tree/main/i18n)
* [लॉगिन मॉड्यूल आस्तै भाशा पैक](https://github.com/wacpkg/user/tree/main/ui.i18n)
* [वेबसाइट बहुभाषी दस्तावेजीकरण](https://github.com/xxai-doc)

फ्रंट-एंड प्रोग्रामिंग लैंग्वेज [@w5/coffee_plus](http://npmjs.com/@w5/coffee_plus) ऐ , जेह् ड़ी कॉफीस्क्रिप्ट सिंटैक्स दे आधार उप्पर किश फीचर जोड़दी ऐ , दिक्खो [./coffee_plus.md](./coffee_plus.md) .

## वेबसाइटें ते दस्तावेजें दा अंतर्राष्ट्रीयकरण

निम्नलिखित 3 प्रोजेक्टें पर निर्माण करो

* [@ w5/mdt ने दी](https://www.npmjs.com/package/@w5/mdt)

  प्रत्यय `.mdt` ऐ , तुस बाहरी फाइलें दा संदर्भ देने आस्तै `<+ ./coffee_plus/import.js>` दे समान वाक्य रचना दा इस्तेमाल करी सकदे ओ , ते `.md` प्रत्यय कन्नै मार्कडाउन पैदा करी सकदे ओ .

* [@ w5/trmd ऐ](https://www.npmjs.com/package/@w5/trmd)

  मार्कडाउन अनुवाद कोड ते लिंक दा अनुवाद नेईं करग, ते अनुवादित वाक्यें गी कैश करग। जेकर अनुवाद च संशोधन कीता गेदा ऐ पर मूल पाठ च संशोधन नेईं कीता गेदा ऐ तां इसगी दुबारा निष्पादत करने कन्नै अनुवाद दे संशोधन गी ओवरराइट नेईं कीता जाग।

* [@ w5/i18n ऐ](https://www.npmjs.com/package/@w5/i18n)

  `yaml` जनरेट कीती गेदी वेबसाइटें दा अनुवाद करने लेई भाशा फाइलें।
