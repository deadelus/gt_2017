# gt_2017
## Sample JSON
```
[
  {
    'repeat(5, 10)': {
      index: '{{index()}}',
      isActive: '{{bool()}}',
      picture: 'http://placehold.it/32x32',
      company: '{{company().toUpperCase()}}',
      phone: '+1 {{phone()}}',
      address: '{{integer(100, 999)}} {{street()}}, {{city()}}, {{state()}}, {{integer(100, 10000)}}',
      about: '{{lorem(1, "paragraphs")}}',
      start: '{{moment(this.date(new Date(2014, 0, 1), new Date())).format("LLLL")}}',
      end: '{{moment(this.date(new Date(2014, 0, 1), new Date())).format("LLLL")}}',
      xp: {'repeat(5, 10)': {name: '{{lorem(1, "paragraphs")}}', lvl: integer(10, 100)}},
      tags: [
        {
          'repeat(5)': '{{lorem(1, "words")}}'
        }
      ]
    }
  }
]
```
