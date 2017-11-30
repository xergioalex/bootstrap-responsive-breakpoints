Boostrap responsive breakpoints
---

Just a tiny configuration for boostrap responsive breakpoints in sass


```
$screen:(
    _xl: 1400px,
    _xl-max: 1399px,
    _xl: 1200px, // $screen-xl
    _xl-max: 1199px, // $screen-xl-max
    _lg: 992px, // $screen-lg
    _lg-max: 991px, // $screen-lg-max
    _md: 768px, // $screen-md
    _md-max: 767px, // $screen-md-max
    _sm: 576px, // $screen-sm
    _sm-max: 575px, // $screen-sm-max
    _xs: 400px, // $screen-xs
    _xs-max: 399px, // $screen-xs-max
);

/*
 * MEDIA QUERYS
 *
 * Tiny grid  devices Phones  (<=400px) = .col-*
 * Extra small grid  devices Phones  (<=576px) = .col-*
 * Small grid  devices Phones  (<=768px) = .col-sm-*
 * Regular grid devices Tablets (≥768px) = .col-md-*
 * Medium grid devices Desktops  (≥992px) = .col-lg-*
 * Large grid devices Desktops  (≥1200px) = .col-xl-*
 * Extra large grid deivces desktop (≥1400px)
 */

// Breakpoint: x >= 1400
@media (min-width: map_get($screen,_xxl)) {

}

// Breakpoint: x <= 1399
@media (max-width: map_get($screen,_xxl-max)) {

}


// Breakpoint: 1200 >= x <= 1399px
@media (min-width: map_get($screen,_xl)) and (max-width: map_get($screen,_xl-max)) {

}

// Breakpoint: x >= 1200
@media (min-width: map_get($screen,_xl)) {

}

// Breakpoint: x <= 1199
@media (max-width: map_get($screen,_xl-max)) {

}

// Breakpoint: 992 >= x <= 1199
@media (min-width: map_get($screen,_lg)) and (max-width: map_get($screen,_xl-max)) {

}

// Breakpoint: x >= 992
@media (min-width: map_get($screen,_lg)) {

}

// Breakpoint: x <= 991
@media (max-width: map_get($screen,_lg-max)) {

}

// Breakpoint: 768 >= x <= 991
@media (min-width: map_get($screen,_md)) and (max-width: map_get($screen,_lg-max)) {

}

// Breakpoint: x <= 767
@media (max-width: map_get($screen,_md-max)) {

}

// Breakpoint: x < 575
@media (max-width: map_get($screen,_sm-max)) {

}

// Breakpoint: x <= 399
@media (max-width: map_get($screen,_xs-max)) {

}
```