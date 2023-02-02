# Ashajyothi
I am pursuing my masters in computer science at northwest missouri state university.i am very passinate to excel in the field of computer science.

![Aboutme](/asha%20photo.jpg)

---

# TRIP

In this table i am  recommend someone visit.
|   **country**  |    **Reason to visit**  |   **Number of days**  |
|----------------|-------------------------|-----------------------|
| Goa            |    exploring beaches    |     8                 |
| chennai        |    to see places        |     2                 |
| kolkata        |    to see buildings     |     5                 |
|hyedarabad      |    to see charminar     |     7                 |

# Pithy Quotes
> So we beat on, boats against the current, borne back ceaselessly into the past. -_Mohan_
>
> The way to get started is to quit talking and begin doing. -_Rahul_

---

# Code Fencing

> How to do Opposite-direction Function?
[Link](https://stackoverflow.com/questions/48532491/how-to-create-loop-for-opposite-or-reverse-classes-in-sass)

Sass
```
@function opposite-direction($directions) {
  $opposite-directions: ();
  $direction-map: (
    'top':    'bottom',
    'right':  'left',
    'bottom': 'top',
    'left':   'right',
    'center': 'center',
    'ltr':    'rtl',
    'rtl':    'ltr'
  );
 
  @each $direction in $directions {
    $direction: to-lower-case($direction);
    
    @if map-has-key($direction-map, $direction) { 
      $opposite-directions: append($opposite-directions, unquote(map-get($direction-map, $direction)));
    } @else {
      @warn "No opposite direction can be found for `#{$direction}`. Direction omitted.";
    }
  }
 
  @return $opposite-directions;
}

[Link](https://css-tricks.com/snippets/sass/opposite-direction-function/)