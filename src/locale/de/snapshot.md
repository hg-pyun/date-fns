# German (de) locale

## `format` and `parse`

| Title                           | Token string | Date                     | `format` result                                  | `parse` result           |
| ------------------------------- | ------------ | ------------------------ | ------------------------------------------------ | ------------------------ |
| Calendar year                   | yo           | 1987-02-11T12:13:14.015Z | 1987.                                            | 1987-01-01T00:00:00.000Z |
|                                 |              | 0005-01-01T12:13:14.015Z | 5.                                               | 0005-01-01T00:00:00.000Z |
| Local week-numbering year       | Yo           | 1987-02-11T12:13:14.015Z | 1987.                                            | 1986-12-29T00:00:00.000Z |
|                                 |              | 0005-01-01T12:13:14.015Z | 4.                                               | 0003-12-29T00:00:00.000Z |
| Quarter (formatting)            | Qo           | 2019-01-01T12:13:14.015Z | 1.                                               | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | 2.                                               | 2019-04-01T00:00:00.000Z |
|                                 | QQQ          | 2019-01-01T12:13:14.015Z | Q1                                               | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | Q2                                               | 2019-04-01T00:00:00.000Z |
|                                 | QQQQ         | 2019-01-01T12:13:14.015Z | 1. Quartal                                       | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | 2. Quartal                                       | 2019-04-01T00:00:00.000Z |
|                                 | QQQQQ        | 2019-01-01T12:13:14.015Z | 1                                                | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | 2                                                | 2019-04-01T00:00:00.000Z |
| Quarter (stand-alone)           | qo           | 2019-01-01T12:13:14.015Z | 1.                                               | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | 2.                                               | 2019-04-01T00:00:00.000Z |
|                                 | qqq          | 2019-01-01T12:13:14.015Z | Q1                                               | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | Q2                                               | 2019-04-01T00:00:00.000Z |
|                                 | qqqq         | 2019-01-01T12:13:14.015Z | 1. Quartal                                       | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | 2. Quartal                                       | 2019-04-01T00:00:00.000Z |
| Month (formatting)              | Mo           | 2019-02-11T12:13:14.015Z | 2.                                               | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | 7.                                               | 2019-07-01T00:00:00.000Z |
|                                 | MMM          | 2019-02-11T12:13:14.015Z | Feb.                                             | Invalid Date             |
|                                 |              | 2019-07-10T12:13:14.015Z | Juli                                             | Invalid Date             |
|                                 | MMMM         | 2019-02-11T12:13:14.015Z | Februar                                          | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | Juli                                             | 2019-07-01T00:00:00.000Z |
|                                 | MMMMM        | 2019-02-11T12:13:14.015Z | F                                                | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | J                                                | 2019-01-01T00:00:00.000Z |
| Month (stand-alone)             | Lo           | 2019-02-11T12:13:14.015Z | 2.                                               | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | 7.                                               | 2019-07-01T00:00:00.000Z |
|                                 | LLL          | 2019-02-11T12:13:14.015Z | Feb.                                             | Invalid Date             |
|                                 |              | 2019-07-10T12:13:14.015Z | Juli                                             | Invalid Date             |
|                                 | LLLL         | 2019-02-11T12:13:14.015Z | Februar                                          | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | Juli                                             | 2019-07-01T00:00:00.000Z |
|                                 | LLLLL        | 2019-02-11T12:13:14.015Z | F                                                | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | J                                                | 2019-01-01T00:00:00.000Z |
| Local week of year              | wo           | 2019-01-01T12:13:14.015Z | 1.                                               | 2018-12-31T00:00:00.000Z |
|                                 |              | 2019-12-01T12:13:14.015Z | 48.                                              | 2019-11-25T00:00:00.000Z |
| ISO week of year                | Io           | 2019-01-01T12:13:14.015Z | 1.                                               | 2018-12-31T00:00:00.000Z |
|                                 |              | 2019-12-01T12:13:14.015Z | 48.                                              | 2019-11-25T00:00:00.000Z |
| Day of month                    | do           | 2019-02-11T12:13:14.015Z | 11.                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-28T12:13:14.015Z | 28.                                              | 2019-02-28T00:00:00.000Z |
| Day of year                     | Do           | 2019-02-11T12:13:14.015Z | 42.                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-12-31T12:13:14.015Z | 365.                                             | 2019-12-31T00:00:00.000Z |
| Day of week (formatting)        | E            | 2019-02-11T12:13:14.015Z | Mo.                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | Fr.                                              | 2019-02-15T00:00:00.000Z |
|                                 | EE           | 2019-02-11T12:13:14.015Z | Mo.                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | Fr.                                              | 2019-02-15T00:00:00.000Z |
|                                 | EEE          | 2019-02-11T12:13:14.015Z | Mo.                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | Fr.                                              | 2019-02-15T00:00:00.000Z |
|                                 | EEEE         | 2019-02-11T12:13:14.015Z | Montag                                           | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | Freitag                                          | 2019-02-15T00:00:00.000Z |
|                                 | EEEEE        | 2019-02-11T12:13:14.015Z | M                                                | Invalid Date             |
|                                 |              | 2019-02-15T12:13:14.015Z | F                                                | 2019-02-15T00:00:00.000Z |
|                                 | EEEEEE       | 2019-02-11T12:13:14.015Z | Mo                                               | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | Fr                                               | 2019-02-15T00:00:00.000Z |
| ISO day of week (formatting)    | io           | 2019-02-11T12:13:14.015Z | 1.                                               | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 5.                                               | 2019-02-15T00:00:00.000Z |
|                                 | iii          | 2019-02-11T12:13:14.015Z | Mo.                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | Fr.                                              | 2019-02-15T00:00:00.000Z |
|                                 | iiii         | 2019-02-11T12:13:14.015Z | Montag                                           | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | Freitag                                          | 2019-02-15T00:00:00.000Z |
|                                 | iiiii        | 2019-02-11T12:13:14.015Z | M                                                | Invalid Date             |
|                                 |              | 2019-02-15T12:13:14.015Z | F                                                | 2019-02-15T00:00:00.000Z |
|                                 | iiiiii       | 2019-02-11T12:13:14.015Z | Mo                                               | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | Fr                                               | 2019-02-15T00:00:00.000Z |
| Local day of week (formatting)  | eo           | 2019-02-11T12:13:14.015Z | 1.                                               | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 5.                                               | 2019-02-15T00:00:00.000Z |
|                                 | eee          | 2019-02-11T12:13:14.015Z | Mo.                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | Fr.                                              | 2019-02-15T00:00:00.000Z |
|                                 | eeee         | 2019-02-11T12:13:14.015Z | Montag                                           | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | Freitag                                          | 2019-02-15T00:00:00.000Z |
|                                 | eeeee        | 2019-02-11T12:13:14.015Z | M                                                | Invalid Date             |
|                                 |              | 2019-02-15T12:13:14.015Z | F                                                | 2019-02-15T00:00:00.000Z |
|                                 | eeeeee       | 2019-02-11T12:13:14.015Z | Mo                                               | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | Fr                                               | 2019-02-15T00:00:00.000Z |
| Local day of week (stand-alone) | co           | 2019-02-11T12:13:14.015Z | 1.                                               | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 5.                                               | 2019-02-15T00:00:00.000Z |
|                                 | ccc          | 2019-02-11T12:13:14.015Z | Mo.                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | Fr.                                              | 2019-02-15T00:00:00.000Z |
|                                 | cccc         | 2019-02-11T12:13:14.015Z | Montag                                           | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | Freitag                                          | 2019-02-15T00:00:00.000Z |
|                                 | ccccc        | 2019-02-11T12:13:14.015Z | M                                                | Invalid Date             |
|                                 |              | 2019-02-15T12:13:14.015Z | F                                                | 2019-02-15T00:00:00.000Z |
|                                 | cccccc       | 2019-02-11T12:13:14.015Z | Mo                                               | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | Fr                                               | 2019-02-15T00:00:00.000Z |
| AM, PM                          | a            | 2019-02-11T11:13:14.015Z | vorm.                                            | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | nachm.                                           | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | nachm.                                           | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | vorm.                                            | 2019-02-11T00:00:00.000Z |
|                                 | aa           | 2019-02-11T11:13:14.015Z | vorm.                                            | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | nachm.                                           | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | nachm.                                           | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | vorm.                                            | 2019-02-11T00:00:00.000Z |
|                                 | aaa          | 2019-02-11T11:13:14.015Z | vorm.                                            | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | nachm.                                           | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | nachm.                                           | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | vorm.                                            | 2019-02-11T00:00:00.000Z |
|                                 | aaaa         | 2019-02-11T11:13:14.015Z | vormittags                                       | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | nachmittags                                      | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | nachmittags                                      | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | vormittags                                       | 2019-02-11T00:00:00.000Z |
|                                 | aaaaa        | 2019-02-11T11:13:14.015Z | vm.                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | nm.                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | nm.                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | vm.                                              | 2019-02-11T00:00:00.000Z |
| AM, PM, noon, midnight          | b            | 2019-02-11T11:13:14.015Z | vorm.                                            | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | nachm.                                           | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | nachm.                                           | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | vorm.                                            | 2019-02-11T00:00:00.000Z |
|                                 | bb           | 2019-02-11T11:13:14.015Z | vorm.                                            | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | nachm.                                           | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | nachm.                                           | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | vorm.                                            | 2019-02-11T00:00:00.000Z |
|                                 | bbb          | 2019-02-11T11:13:14.015Z | vorm.                                            | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | nachm.                                           | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | nachm.                                           | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | vorm.                                            | 2019-02-11T00:00:00.000Z |
|                                 | bbbb         | 2019-02-11T11:13:14.015Z | vormittags                                       | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | nachmittags                                      | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | nachmittags                                      | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | vormittags                                       | 2019-02-11T00:00:00.000Z |
|                                 | bbbbb        | 2019-02-11T11:13:14.015Z | vm.                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | nm.                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | nm.                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | vm.                                              | 2019-02-11T00:00:00.000Z |
| Flexible day period             | B            | 2019-02-11T11:13:14.015Z | morgens                                          | 2019-02-11T04:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | nachmittags                                      | Invalid Date             |
|                                 |              | 2019-02-11T19:13:14.015Z | abends                                           | 2019-02-11T17:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | nachts                                           | 2019-02-11T12:00:00.000Z |
|                                 | BB           | 2019-02-11T11:13:14.015Z | morgens                                          | 2019-02-11T04:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | nachmittags                                      | Invalid Date             |
|                                 |              | 2019-02-11T19:13:14.015Z | abends                                           | 2019-02-11T17:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | nachts                                           | 2019-02-11T12:00:00.000Z |
|                                 | BBB          | 2019-02-11T11:13:14.015Z | morgens                                          | 2019-02-11T04:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | nachmittags                                      | Invalid Date             |
|                                 |              | 2019-02-11T19:13:14.015Z | abends                                           | 2019-02-11T17:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | nachts                                           | 2019-02-11T12:00:00.000Z |
|                                 | BBBB         | 2019-02-11T11:13:14.015Z | morgens                                          | 2019-02-11T04:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | nachmittags                                      | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | abends                                           | 2019-02-11T17:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | nachts                                           | 2019-02-11T12:00:00.000Z |
|                                 | BBBBB        | 2019-02-11T11:13:14.015Z | morgens                                          | 2019-02-11T04:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | nachm.                                           | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | abends                                           | 2019-02-11T17:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | nachts                                           | 2019-02-11T12:00:00.000Z |
| Hour [1-12]                     | ho           | 2019-02-11T11:13:14.015Z | 11.                                              | 2019-02-11T11:00:00.000Z |
|                                 |              | 2019-02-11T23:13:14.015Z | 11.                                              | 2019-02-11T23:00:00.000Z |
| Hour [0-23]                     | Ho           | 2019-02-11T11:13:14.015Z | 11.                                              | 2019-02-11T11:00:00.000Z |
|                                 |              | 2019-02-11T23:13:14.015Z | 23.                                              | 2019-02-11T23:00:00.000Z |
| Hour [0-11]                     | Ko           | 2019-02-11T11:13:14.015Z | 11.                                              | 2019-02-11T11:00:00.000Z |
|                                 |              | 2019-02-11T23:13:14.015Z | 11.                                              | 2019-02-11T23:00:00.000Z |
| Hour [1-24]                     | ko           | 2019-02-11T11:13:14.015Z | 11.                                              | 2019-02-11T11:00:00.000Z |
|                                 |              | 2019-02-11T23:13:14.015Z | 23.                                              | 2019-02-11T23:00:00.000Z |
| Minute                          | mo           | 2019-01-01T12:01:14.015Z | 1.                                               | 2019-01-01T12:01:00.000Z |
|                                 |              | 2019-04-01T12:55:14.015Z | 55.                                              | 2019-04-01T12:55:00.000Z |
| Second                          | so           | 2019-01-01T12:13:01.015Z | 1.                                               | 2019-01-01T12:13:01.000Z |
|                                 |              | 2019-04-01T12:13:55.015Z | 55.                                              | 2019-04-01T12:13:55.000Z |
| Long localized date             | P            | 1987-02-11T12:13:14.015Z | 11.02.1987                                       | 1987-02-11T00:00:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 29.05.1453                                       | 1453-05-29T00:00:00.000Z |
|                                 | PP           | 1987-02-11T12:13:14.015Z | 11. Feb. 1987                                    | Invalid Date             |
|                                 |              | 1453-05-29T23:59:59.999Z | 29. Mai 1453                                     | 1453-05-29T00:00:00.000Z |
|                                 | PPP          | 1987-02-11T12:13:14.015Z | 11. Februar 1987                                 | 1987-02-11T00:00:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 29. Mai 1453                                     | 1453-05-29T00:00:00.000Z |
|                                 | PPPP         | 1987-02-11T12:13:14.015Z | Mittwoch, 11. Februar 1987                       | 1987-02-11T00:00:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | Sonntag, 29. Mai 1453                            | 1453-05-29T00:00:00.000Z |
| Long localized time             | p            | 1987-02-11T12:13:14.015Z | 12:13                                            | 1987-02-11T12:13:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 23:59                                            | 1453-05-29T23:59:00.000Z |
|                                 | pp           | 1987-02-11T12:13:14.015Z | 12:13:14                                         | 1987-02-11T12:13:14.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 23:59:59                                         | 1453-05-29T23:59:59.000Z |
|                                 | ppp          | 1987-02-11T12:13:14.015Z | 12:13:14 GMT+0                                   | Errored                  |
|                                 |              | 1453-05-29T23:59:59.999Z | 23:59:59 GMT+0                                   | Errored                  |
|                                 | pppp         | 1987-02-11T12:13:14.015Z | 12:13:14 GMT+00:00                               | Errored                  |
|                                 |              | 1453-05-29T23:59:59.999Z | 23:59:59 GMT+00:00                               | Errored                  |
| Combination of date and time    | Pp           | 1987-02-11T12:13:14.015Z | 11.02.1987 12:13                                 | 1987-02-11T12:13:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 29.05.1453 23:59                                 | 1453-05-29T23:59:00.000Z |
|                                 | PPpp         | 1987-02-11T12:13:14.015Z | 11. Feb. 1987 12:13:14                           | Invalid Date             |
|                                 |              | 1453-05-29T23:59:59.999Z | 29. Mai 1453 23:59:59                            | 1453-05-29T23:59:59.000Z |
|                                 | PPPppp       | 1987-02-11T12:13:14.015Z | 11. Februar 1987 um 12:13:14 GMT+0               | Errored                  |
|                                 |              | 1453-05-29T23:59:59.999Z | 29. Mai 1453 um 23:59:59 GMT+0                   | Errored                  |
|                                 | PPPPpppp     | 1987-02-11T12:13:14.015Z | Mittwoch, 11. Februar 1987 um 12:13:14 GMT+00:00 | Errored                  |
|                                 |              | 1453-05-29T23:59:59.999Z | Sonntag, 29. Mai 1453 um 23:59:59 GMT+00:00      | Errored                  |

## `formatDistance`

If now is January 1st, 2000, 00:00.

| Date                     | Result               | `includeSeconds: true`  | `addSuffix: true`        |
| ------------------------ | -------------------- | ----------------------- | ------------------------ |
| 2006-01-01T00:00:00.000Z | etwa 6 Jahre         | etwa 6 Jahre            | in etwa 6 Jahren         |
| 2005-01-01T00:00:00.000Z | etwa 5 Jahre         | etwa 5 Jahre            | in etwa 5 Jahren         |
| 2004-01-01T00:00:00.000Z | etwa 4 Jahre         | etwa 4 Jahre            | in etwa 4 Jahren         |
| 2003-01-01T00:00:00.000Z | etwa 3 Jahre         | etwa 3 Jahre            | in etwa 3 Jahren         |
| 2002-01-01T00:00:00.000Z | etwa 2 Jahre         | etwa 2 Jahre            | in etwa 2 Jahren         |
| 2001-06-01T00:00:00.000Z | mehr als 1 Jahr      | mehr als 1 Jahr         | in mehr als 1 Jahr       |
| 2001-02-01T00:00:00.000Z | etwa 1 Jahr          | etwa 1 Jahr             | in etwa 1 Jahr           |
| 2001-01-01T00:00:00.000Z | etwa 1 Jahr          | etwa 1 Jahr             | in etwa 1 Jahr           |
| 2000-06-01T00:00:00.000Z | 5 Monate             | 5 Monate                | in 5 Monaten             |
| 2000-03-01T00:00:00.000Z | 2 Monate             | 2 Monate                | in 2 Monaten             |
| 2000-02-01T00:00:00.000Z | etwa 1 Monat         | etwa 1 Monat            | in etwa 1 Monat          |
| 2000-01-15T00:00:00.000Z | 14 Tage              | 14 Tage                 | in 14 Tagen              |
| 2000-01-02T00:00:00.000Z | 1 Tag                | 1 Tag                   | in 1 Tag                 |
| 2000-01-01T06:00:00.000Z | etwa 6 Stunden       | etwa 6 Stunden          | in etwa 6 Stunden        |
| 2000-01-01T01:00:00.000Z | etwa 1 Stunde        | etwa 1 Stunde           | in etwa 1 Stunde         |
| 2000-01-01T00:45:00.000Z | etwa 1 Stunde        | etwa 1 Stunde           | in etwa 1 Stunde         |
| 2000-01-01T00:30:00.000Z | 30 Minuten           | 30 Minuten              | in 30 Minuten            |
| 2000-01-01T00:15:00.000Z | 15 Minuten           | 15 Minuten              | in 15 Minuten            |
| 2000-01-01T00:01:00.000Z | 1 Minute             | 1 Minute                | in 1 Minute              |
| 2000-01-01T00:00:25.000Z | weniger als 1 Minute | halbe Minute            | in weniger als 1 Minute  |
| 2000-01-01T00:00:15.000Z | weniger als 1 Minute | weniger als 20 Sekunden | in weniger als 1 Minute  |
| 2000-01-01T00:00:05.000Z | weniger als 1 Minute | weniger als 10 Sekunden | in weniger als 1 Minute  |
| 2000-01-01T00:00:00.000Z | weniger als 1 Minute | weniger als 5 Sekunden  | vor weniger als 1 Minute |
| 1999-12-31T23:59:55.000Z | weniger als 1 Minute | weniger als 10 Sekunden | vor weniger als 1 Minute |
| 1999-12-31T23:59:45.000Z | weniger als 1 Minute | weniger als 20 Sekunden | vor weniger als 1 Minute |
| 1999-12-31T23:59:35.000Z | weniger als 1 Minute | halbe Minute            | vor weniger als 1 Minute |
| 1999-12-31T23:59:00.000Z | 1 Minute             | 1 Minute                | vor 1 Minute             |
| 1999-12-31T23:45:00.000Z | 15 Minuten           | 15 Minuten              | vor 15 Minuten           |
| 1999-12-31T23:30:00.000Z | 30 Minuten           | 30 Minuten              | vor 30 Minuten           |
| 1999-12-31T23:15:00.000Z | etwa 1 Stunde        | etwa 1 Stunde           | vor etwa 1 Stunde        |
| 1999-12-31T23:00:00.000Z | etwa 1 Stunde        | etwa 1 Stunde           | vor etwa 1 Stunde        |
| 1999-12-31T18:00:00.000Z | etwa 6 Stunden       | etwa 6 Stunden          | vor etwa 6 Stunden       |
| 1999-12-30T00:00:00.000Z | 2 Tage               | 2 Tage                  | vor 2 Tagen              |
| 1999-12-15T00:00:00.000Z | 17 Tage              | 17 Tage                 | vor 17 Tagen             |
| 1999-12-01T00:00:00.000Z | etwa 1 Monat         | etwa 1 Monat            | vor etwa 1 Monat         |
| 1999-11-01T00:00:00.000Z | 2 Monate             | 2 Monate                | vor 2 Monaten            |
| 1999-06-01T00:00:00.000Z | 7 Monate             | 7 Monate                | vor 7 Monaten            |
| 1999-01-01T00:00:00.000Z | etwa 1 Jahr          | etwa 1 Jahr             | vor etwa 1 Jahr          |
| 1998-12-01T00:00:00.000Z | etwa 1 Jahr          | etwa 1 Jahr             | vor etwa 1 Jahr          |
| 1998-06-01T00:00:00.000Z | mehr als 1 Jahr      | mehr als 1 Jahr         | vor mehr als 1 Jahr      |
| 1998-01-01T00:00:00.000Z | etwa 2 Jahre         | etwa 2 Jahre            | vor etwa 2 Jahren        |
| 1997-01-01T00:00:00.000Z | etwa 3 Jahre         | etwa 3 Jahre            | vor etwa 3 Jahren        |
| 1996-01-01T00:00:00.000Z | etwa 4 Jahre         | etwa 4 Jahre            | vor etwa 4 Jahren        |
| 1995-01-01T00:00:00.000Z | etwa 5 Jahre         | etwa 5 Jahre            | vor etwa 5 Jahren        |
| 1994-01-01T00:00:00.000Z | etwa 6 Jahre         | etwa 6 Jahre            | vor etwa 6 Jahren        |

## `formatDistanceStrict`

If now is January 1st, 2000, 00:00.

| Date                     | Result      | `addSuffix: true` | With forced unit (i.e. `hour`) |
| ------------------------ | ----------- | ----------------- | ------------------------------ |
| 2006-01-01T00:00:00.000Z | 6 Jahre     | in 6 Jahren       | 52608 Stunden                  |
| 2005-01-01T00:00:00.000Z | 5 Jahre     | in 5 Jahren       | 43848 Stunden                  |
| 2004-01-01T00:00:00.000Z | 4 Jahre     | in 4 Jahren       | 35064 Stunden                  |
| 2003-01-01T00:00:00.000Z | 3 Jahre     | in 3 Jahren       | 26304 Stunden                  |
| 2002-01-01T00:00:00.000Z | 2 Jahre     | in 2 Jahren       | 17544 Stunden                  |
| 2001-06-01T00:00:00.000Z | 1 Jahr      | in 1 Jahr         | 12408 Stunden                  |
| 2001-02-01T00:00:00.000Z | 1 Jahr      | in 1 Jahr         | 9528 Stunden                   |
| 2001-01-01T00:00:00.000Z | 1 Jahr      | in 1 Jahr         | 8784 Stunden                   |
| 2000-06-01T00:00:00.000Z | 5 Monate    | in 5 Monaten      | 3648 Stunden                   |
| 2000-03-01T00:00:00.000Z | 2 Monate    | in 2 Monaten      | 1440 Stunden                   |
| 2000-02-01T00:00:00.000Z | 1 Monat     | in 1 Monat        | 744 Stunden                    |
| 2000-01-15T00:00:00.000Z | 14 Tage     | in 14 Tagen       | 336 Stunden                    |
| 2000-01-02T00:00:00.000Z | 1 Tag       | in 1 Tag          | 24 Stunden                     |
| 2000-01-01T06:00:00.000Z | 6 Stunden   | in 6 Stunden      | 6 Stunden                      |
| 2000-01-01T01:00:00.000Z | 1 Stunde    | in 1 Stunde       | 1 Stunde                       |
| 2000-01-01T00:45:00.000Z | 45 Minuten  | in 45 Minuten     | 1 Stunde                       |
| 2000-01-01T00:30:00.000Z | 30 Minuten  | in 30 Minuten     | 1 Stunde                       |
| 2000-01-01T00:15:00.000Z | 15 Minuten  | in 15 Minuten     | 0 Stunden                      |
| 2000-01-01T00:01:00.000Z | 1 Minute    | in 1 Minute       | 0 Stunden                      |
| 2000-01-01T00:00:25.000Z | 25 Sekunden | in 25 Sekunden    | 0 Stunden                      |
| 2000-01-01T00:00:15.000Z | 15 Sekunden | in 15 Sekunden    | 0 Stunden                      |
| 2000-01-01T00:00:05.000Z | 5 Sekunden  | in 5 Sekunden     | 0 Stunden                      |
| 2000-01-01T00:00:00.000Z | 0 Sekunden  | vor 0 Sekunden    | 0 Stunden                      |
| 1999-12-31T23:59:55.000Z | 5 Sekunden  | vor 5 Sekunden    | 0 Stunden                      |
| 1999-12-31T23:59:45.000Z | 15 Sekunden | vor 15 Sekunden   | 0 Stunden                      |
| 1999-12-31T23:59:35.000Z | 25 Sekunden | vor 25 Sekunden   | 0 Stunden                      |
| 1999-12-31T23:59:00.000Z | 1 Minute    | vor 1 Minute      | 0 Stunden                      |
| 1999-12-31T23:45:00.000Z | 15 Minuten  | vor 15 Minuten    | 0 Stunden                      |
| 1999-12-31T23:30:00.000Z | 30 Minuten  | vor 30 Minuten    | 1 Stunde                       |
| 1999-12-31T23:15:00.000Z | 45 Minuten  | vor 45 Minuten    | 1 Stunde                       |
| 1999-12-31T23:00:00.000Z | 1 Stunde    | vor 1 Stunde      | 1 Stunde                       |
| 1999-12-31T18:00:00.000Z | 6 Stunden   | vor 6 Stunden     | 6 Stunden                      |
| 1999-12-30T00:00:00.000Z | 2 Tage      | vor 2 Tagen       | 48 Stunden                     |
| 1999-12-15T00:00:00.000Z | 17 Tage     | vor 17 Tagen      | 408 Stunden                    |
| 1999-12-01T00:00:00.000Z | 1 Monat     | vor 1 Monat       | 744 Stunden                    |
| 1999-11-01T00:00:00.000Z | 2 Monate    | vor 2 Monaten     | 1464 Stunden                   |
| 1999-06-01T00:00:00.000Z | 7 Monate    | vor 7 Monaten     | 5136 Stunden                   |
| 1999-01-01T00:00:00.000Z | 1 Jahr      | vor 1 Jahr        | 8760 Stunden                   |
| 1998-12-01T00:00:00.000Z | 1 Jahr      | vor 1 Jahr        | 9504 Stunden                   |
| 1998-06-01T00:00:00.000Z | 2 Jahre     | vor 2 Jahren      | 13896 Stunden                  |
| 1998-01-01T00:00:00.000Z | 2 Jahre     | vor 2 Jahren      | 17520 Stunden                  |
| 1997-01-01T00:00:00.000Z | 3 Jahre     | vor 3 Jahren      | 26280 Stunden                  |
| 1996-01-01T00:00:00.000Z | 4 Jahre     | vor 4 Jahren      | 35064 Stunden                  |
| 1995-01-01T00:00:00.000Z | 5 Jahre     | vor 5 Jahren      | 43824 Stunden                  |
| 1994-01-01T00:00:00.000Z | 6 Jahre     | vor 6 Jahren      | 52584 Stunden                  |

## `formatRelative`

If now is January 1st, 2000, 00:00.

| Date                     | Result                  |
| ------------------------ | ----------------------- |
| 2000-01-10T00:00:00.000Z | 10.01.2000              |
| 2000-01-05T00:00:00.000Z | Mittwoch um 00:00       |
| 2000-01-02T00:00:00.000Z | morgen um 00:00         |
| 2000-01-01T00:00:00.000Z | heute um 00:00          |
| 1999-12-31T00:00:00.000Z | gestern um 00:00        |
| 1999-12-27T00:00:00.000Z | letzten Montag um 00:00 |
| 1999-12-21T00:00:00.000Z | 21.12.1999              |