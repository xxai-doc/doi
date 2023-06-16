<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

एह् सलाह दित्ती जंदी ऐ जे पैह् ले nodejs, [direnv](https://direnv.net) , [bun गी](https://github.com/oven-sh/bun) इंस्टॉल करो, ते फिर डायरेक्टरी च दाखल होने दे बाद `direnv allow` ( डायरेक्टरी च दाखल होने दे बाद [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) स्वतः निष्पादत होई जाग)।

मतलब ऐ: चीनी अनुवाद जापानी, कोरियाई, अंग्रेजी, अंग्रेजी अनुवाद बाकी सारी भाशाएं च। अगर तुस सिर्फ चीनी ते अंग्रेजी दा समर्थन करना चांदे ओ तां तुस सिर्फ `zh: en` लिखी सकदे ओ।

मतलब ऐ: चीनी अनुवाद जापानी, कोरियाई, अंग्रेजी, अंग्रेजी अनुवाद बाकी सारी भाशाएं च। अगर तुस सिर्फ चीनी ते अंग्रेजी दा समर्थन करना चांदे ओ तां तुस सिर्फ `zh: en` लिखी सकदे ओ।

* [फ्रंट-एंड कोड](https://github.com/xxai-art/web)
* [समग्र रूप कन्नै साइट आस्तै भाशा पैक](https://github.com/xxai-art/web/tree/main/i18n)
* [लॉगिन मॉड्यूल आस्तै भाशा पैक](https://github.com/wacpkg/user/tree/main/ui.i18n)
* [वेबसाइट बहुभाषी दस्तावेजीकरण](https://github.com/xxai-doc)

फ्रंट-एंड प्रोग्रामिंग लैंग्वेज [@w5/coffee_plus](http://npmjs.com/@w5/coffee_plus) ऐ , जेह् ड़ी कॉफीस्क्रिप्ट सिंटैक्स दे आधार उप्पर किश फीचर जोड़दी ऐ , दिक्खो [./coffee_plus.md](./coffee_plus.md) .

## वेबसाइटें ते दस्तावेजें दा अंतर्राष्ट्रीयकरण

निम्नलिखित 3 प्रोजेक्टें पर निर्माण करो

* [@ w5/mdt दा](https://www.npmjs.com/package/@w5/mdt)

  प्रत्यय `.mdt` ऐ , तुस बाहरी फाइलें दा संदर्भ देने आस्तै `<+ ./coffee_plus/import.js>` दे समान वाक्य रचना दा इस्तेमाल करी सकदे ओ , ते `.md` प्रत्यय कन्नै मार्कडाउन पैदा करी सकदे ओ .

* [@ w5/trmd ऐ](https://www.npmjs.com/package/@w5/trmd)

  मार्कडाउन अनुवाद कोड ते लिंक दा अनुवाद नेईं करग, ते अनुवादित वाक्यें गी कैश करग। जेकर अनुवाद च संशोधन कीता गेदा ऐ पर मूल पाठ च संशोधन नेईं कीता गेदा ऐ तां इसगी दुबारा निष्पादत करने कन्नै अनुवाद दे संशोधन गी ओवरराइट नेईं कीता जाग।

* [@ w5/i18n ऐ](https://www.npmjs.com/package/@w5/i18n)

  `yaml` जनरेट कीती गेदी वेबसाइटें दा अनुवाद करने लेई भाशा फाइलें।

### दस्तावेज अनुवाद स्वचालन निर्देश

कोड भंडार [xxai-art/doc](https://github.com/xxai-art/doc) दिक्खो

एह् सलाह दित्ती जंदी ऐ जे पैह् ले nodejs, [direnv](https://direnv.net) , [bun गी](https://github.com/oven-sh/bun) इंस्टॉल करो, ते फिर डायरेक्टरी च दाखल होने दे बाद `direnv allow` ( डायरेक्टरी च दाखल होने दे बाद [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) स्वतः निष्पादत होई जाग)।

सैकड़ें भाशाएं च अनुवाद कीते गेदे बड्डे कोड बेस थमां बचने आस्तै, मैं हर भाशा आस्तै इक बक्खरा कोड बेस बनाया ते कोड बेस गी संग्रहीत करने आस्तै इक संगठन बनाया

वातावरण चर `GITHUB_ACCESS_TOKEN` सेट करने ते फ्ही [create.github.coffee](https://github.com/xxai-art/doc/blob/main/create.github.coffee) चलाने कन्नै कोड भंडार स्वतः बनाई जाग.

बेशक, तुस इसगी कोड बेस च बी पाई सकदे ओ।

अनुवाद स्क्रिप्ट संदर्भ [run.sh](https://github.com/xxai-art/doc/blob/main/run.sh)

स्क्रिप्ट कोड दी व्याख्या इस चाल्ली कीती जंदी ऐ:

[bunx](https://bun.sh/docs/cli/bunx) npx दा इक प्रतिस्थापन ऐ, जेह् ड़ा तेज़ ऐ। बेशक, जेकर तुंदे कोल बन इंस्टॉल नेईं ऐ तां तुस इसदे बजाय `npx` इस्तेमाल करी सकदे ओ.

`bunx mdt zh` zh डायरेक्टरी च `.mdt` `.md` दे रूप च रेंडर करदा ऐ , थल्ले 2 लिंक कीती गेदी फाइलें गी दिक्खो

* [कॉफी_प्लस.एमडीटी](https://github.com/xxai-doc/zh/blob/main/coffee_plus.mdt)
* [कॉफी_प्लस.एमडी](https://github.com/xxai-doc/zh/blob/main/coffee_plus.md)

`bunx i18n` अनुवाद आस्तै कोर कोड ऐ (जेकर तुंदे कोल सिर्फ `nodejs` इंस्टॉल न, पर `bun` ते `direnv` इंस्टॉल नेईं न, तां तुस अनुवाद करने आस्तै `npx i18n` गी बी चला सकदे ओ)।

एह् [i18n.yml गी](https://github.com/xxai-art/doc/blob/main/i18n.yml) पार्स करग , इस दस्तावेज़ च `i18n.yml` दा कॉन्फ़िगरेशन इस चाल्ली ऐ :

```
en:
zh: ja ko en
```

मतलब ऐ: चीनी अनुवाद जापानी, कोरियाई, अंग्रेजी, अंग्रेजी अनुवाद बाकी सारी भाशाएं च। अगर तुस सिर्फ चीनी ते अंग्रेजी दा समर्थन करना चांदे ओ तां तुस सिर्फ `zh: en` लिखी सकदे ओ।

आखरी [gen.README.coffee](https://github.com/xxai-art/doc/blob/main/gen.README.coffee) ऐ , जेह् ड़ा हर भाशा दे `README.md` दे मुक्ख शीर्शक ते पैह् ले उपशीर्षक दे बश्कार सामग्री गी कड्ढदा ऐ तां जे इक प्रविश्टी `README.md` पैदा कीती जाई सकै. कोड बड़ा सरल ऐ, तुस अपने आपै गी दिक्खी सकदे ओ।

मुफ्त अनुवाद आस्तै गूगल एपीआई दा इस्तेमाल कीता जंदा ऐ। जेकर तुस Google गी एक्सेस नेईं करी सकदे ओ तां कृपा करियै इक प्रॉक्सी कॉन्फ़िगर ते सेट करो, जि’यां:

```
export https_proxy=http://127.0.0.1:7890 http_proxy=http://127.0.0.1:7890 all_proxy=socks5://127.0.0.1:7890
```

अनुवाद स्क्रिप्ट `.i18n` डायरेक्टरी च इक अनुवादित कैशे पैदा करग, कृपा करियै इसगी `git status` कन्नै जांच करो ते बार-बार अनुवादें थमां बचने आस्तै कोड भंडार च जोड़ो.

कृपा करियै हर बारी जेकर तुस कैशे गी अपडेट करने आस्तै अनुवाद गी संशोधित करदे ओ तां `bunx i18n` चलाओ.

जेकर मूल पाठ ते अनुवाद इक गै समें च संशोधित कीते गेदे न तां कैशे च भ्रम पैदा होई जाग, इसलेई जेकर तुस संशोधित करना चांह् दे ओ तां तुस सिर्फ इक गै संशोधित करी सकदे ओ, ते फ्ही कैशे गी अपडेट करने आस्तै `bunx i18n` चलाओ.
