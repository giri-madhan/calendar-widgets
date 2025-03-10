---
title: listDaysInMonth
slug: /helpers/listDaysInMonth
---

# `listDaysInMonth`

The `listDaysInMonth` function generates an array of formatted date strings representing each day in a given month and year.

## Syntax

```ts
import {listDaysInMonth} from 'calendar-widgets';

listDaysInMonth(year: string, month: string);
```

## Parameters
The function takes the following parameters:

- `year` - Required. An integer representing the year for which to generate the list of days, between 1900 and 2100.
- `month` - Required. An integer representing the month for which to generate the list of days, between 1 and 12.

## Return Value

The function returns an array of formatted date strings representing each day in the specified month and year.

## Errors

The function throws an error if the month parameter is not a valid month between 1 and 12, or if the year parameter is not a valid year between 1900 and 2100.

## Usage Example

```js
import { listDaysInMonth } from 'calendar-widgets';

const daysInFebruary2023 = listDaysInMonth(2023, 2);
console.log(daysInFebruary2023);
/*
Output:
[
  "02/01/2023",
  "02/02/2023",
  "02/03/2023",
  // ...and so on for the remaining days
  "02/28/2023"
]
*/
```