# Notes on Flexbox Froggy

In CSS you have ```Property: Value;``` 

**All the alignment and justification is done on the container**

**All of these actions must start first with the ```display: flex;``` then you start aligning and justifying**

```justify-content``` property which aligns items **horizontally**,  takes the following values- 

1. ```flex-start```: aligns to right or start
1. ```flex-end```: aligns to left or end
1. ```center```: middle or center
1. ```space-between```: Displays multiple items with equal spaces **between** them. Will have greater space between the items. At the end (left-right) there will be no space
1. ```space-around```: Displays multiple item with equal spaces **around** them. Balanced spaces all the way around the items. The spaces in the outside will be equal to that in the inside


```align-items``` aligns stuff **vertically** and accepts the following the values -

1. ```flex-start```: Items aligned at the top or start
1. ```flex-end```: Items aligned at the bottom or end
1. ```center```: Items aligned at the center
1. ```baseline```: Items aligned at the baseline
1. ```stretch```: Items are streched to fit


```flex-direction``` determines the dirctions of the items within the container. It might mess up the structure so use it justify and align properties. Like having a reverse direction will require you to be counterintuitive with justify and align properties, so start will become end. It takes the following values -


1. ```row```: Items are placed in rows
1. ```row-reverse```: Items are placed in reverse row order
1. ```column```: Items are placed in column vertically
1. ```column-reverse```: Reverse column structure


```order``` is a item specific proerty helps you structure the directions of specific items in a container and it is much more versatile than flex-direction. By default the order is 0. But it can also take in negative numbers (-2, -1, 0, 1, 2). It shifts others items. The syntax ```order: 2```. Don't take as positional or index value, rather than it is the order of direction.


```align-self``` is also a item specific property which takes the same values as align-items to align itself within the container.


```flex-wrap``` deals with wrapping and fitting items in a container. Eliminates squeezing. Takes the following values -

1. ```nowrap```: No wrap or no second lines. All items fit together or squeezed together in one single line
1. ```wrap```: Items wrap around in addiotional lines. As many lines it takes
1. ```wrap-reverse```: Wraps items in additional but reversely


```flex-flow``` is the combination of flex-direction and flex-wrap. It accepts each values for the properties with a space in between them. Like ```flex-flow: row wrap```

```align-content``` not to be confused with align-items, determines line spacing when it is wrapped. It deals with spaces between the lines when the flex-wrap is set to wrap. The values it takes are-

1. ```flex-start```: Minimum gap between lines. Items are all at the top
1. ```flex-end```: Minimum gap, items at the bottom
1. ```center```: Minimum gap, center
1. ```space-around```: Uniform gaps around the lines
1. ```space-between```: No gaps end to end of the line. Gap in the middle.
1. ```stretch```: Lines are steched to fit the container



## Solutions

### Level 24

```
flex-flow: column-reverse wrap-reverse;
align-content: space-between;
justify-content: center
```
