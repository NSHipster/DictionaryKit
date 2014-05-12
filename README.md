# DictionaryKit

**An Objective-C Wrapper for _Private_ Dictionary Services on Mac OS X**

> This library accesses private OS X APIs, making it unsuitable for apps submitted to the App Store.

## Usage

```objective-c
#import "DictionaryKit.h"

TTTDictionary *dictionary = [TTTDictionary dictionaryNamed:DCSOxfordEnglishDictionary];
NSLog(@"%@\n", dictionary.name);

NSString *term = @"apple";
for (TTTDictionaryEntry *entry in [dictionary entriesForSearchTerm:term]) {
    NSLog(@"%@", entry.text);
}
```

## Available Dictionaries

~~~{objective-c}
NSString * const DCSAppleDictionaryName = @"Apple Dictionary";
NSString * const DCSDutchDictionaryName = @"Prisma woordenboek Nederlands";
NSString * const DCSFrenchDictionaryName = @"Multidictionnaire de la langue française";
NSString * const DCSGermanDictionaryName = @"Duden-Wissensnetz deutsche Sprache";
NSString * const DCSItalianDictionaryName = @"Dizionario italiano da un affiliato di Oxford University Press";
NSString * const DCSJapaneseSupaDaijirinDictionaryName = @"スーパー大辞林";
NSString * const DCSJapanese_EnglishDictionaryName = @"ウィズダム英和辞典 / ウィズダム和英辞典";
NSString * const DCSKoreanDictionaryName = @"New Ace Korean Language Dictionary";
NSString * const DCSKorean_EnglishDictionaryName = @"New Ace English-Korean Dictionary and New Ace Korean-English Dictionary";
NSString * const DCSNewOxfordAmericanDictionaryName = @"New Oxford American Dictionary";
NSString * const DCSOxfordAmericanWritersThesaurus = @"Oxford American Writer's Thesaurus";
NSString * const DCSOxfordDictionaryOfEnglish = @"Oxford Dictionary of English";
NSString * const DCSOxfordThesaurusOfEnglish = @"Oxford Thesaurus of English";
NSString * const DCSSimplifiedChineseDictionaryName = @"现代汉语规范词典";
NSString * const DCSSimplifiedChinese_EnglishDictionaryName = @"Oxford Chinese Dictionary";
NSString * const DCSSpanishDictionaryName = @"Diccionario General de la Lengua Española Vox";
NSString * const DCSWikipediaDictionaryName = @"Wikipedia";
~~~

### Contact

[Mattt Thompson](http://github.com/mattt)
[@mattt](https://twitter.com/mattt)

## License

DictionaryKit is available under the MIT license. See the LICENSE file for more info.
