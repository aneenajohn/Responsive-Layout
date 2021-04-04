# Responsive Layout

## Day 01: Using percentages & avoiding heights
### Percentages Vs Fixed widths

 >*By default, things are responsive.*

 Unless and until we dont assign a fixed width to any element our website is responsive.
 Whenever we try to create layouts for website, we create a problem by taking the responsiveness away.
 Then, we try to solve this problem by defining media queries for different screen sizes.

### So, how can we fix this problem?
As said earlier, "By default, things are responsive", which means that every element has a width of 100% of its parent.So, irrespective of the screen size, it is always 100% of viewport.
Hence, we can make our life easier and pretty simple by giving width in terms of % values instead of a fixed value.

### Percentages on the child.

```
<body>
    <div class="parent">
        <div class="child">
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. 
            Nesciunt nam ullam quo incidunt rerum corporis reprehenderit blanditiis natus quae consequatur,    
            possimus, dolores, mollitia a quis temporibus eos ut similique cupiditate!
        </div>
    </div>
</body>
```

When you give the parent, `width:80%` and the child `width:50%`, __what does it actually mean?__**
```
.parent{
     width:80%;
     }
     
.child{
    width:50%;
    }
```

The parent class would have 80% of its parent (ie) body and the child class would have 50% of width of its parent (ie) 50% of the 80% given to the parent.
>* The bigger the parent gets, the bigger the child gets.
>* The smaller the child gets, the smaller the child gets.
>* It's always the relation between them.



