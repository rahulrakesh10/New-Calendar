
# React Continuous Calendar

Continuous Calendar is a bare-bones calendar built with React and Tailwindcss. It does not include event creation and display, as that's left up to your discretion.

### [Live Demo](https://continuous-calendar.vercel.app/)

### So what does it do? ✨

- Displays 12 months at once, with respect to the specified year.
- Allows for quick-navigation to specific months and Today.
- Clicking on a cell triggers the onClick event with (day, month, year).
- Responsive; supports mobile, tablet, and desktop views.


### Installation 💻

There is no npm package, it's just 1 file you can customize. Simply download or copy the file:

`/components/ContinuousCalendar.tsx`.

Additionally, I have applied the following global css:

```
*:focus:not(ol) {
  @apply outline-none ring-2 ring-cyan-400 border-cyan-400;
}

select {
  -webkit-appearance: none;
  -moz-appearance: none;
  appearance: none;
  text-indent: 1px;
  text-overflow: '';
}

@layer utilities {
  /* Hide scrollbar for Chrome, Safari and Opera */
  .no-scrollbar::-webkit-scrollbar {
    display: none;
  }
  /* Hide scrollbar for IE, Edge and Firefox */
  .no-scrollbar {
    -ms-overflow-style: none;  /* IE and Edge */
    scrollbar-width: none;  /* Firefox */
  }
}
```

### Props ❄️

Prop | Required | Type | Description
--- | --- | --- | --- |
onClick | Optional | `(day:number, month: number, year: number) => void;` | Triggered whenever the user clicks a day on the calendar. |

### Height and Width 🎨

The height and width of the calendar component rely on a parent wrapper. Please refer to `components/DemoWrapper.tsx` as an example of how to structure your React component to achieve your desired calendar size.



