# Sun v Planet

![sunvplanet.png](/Images/sunvplanet.png)    

```netlogo
breed [ suns sun ]
breed [ planets planet ]
to setup
  clear-all
  create-suns 1 [ set color yellow set size 5 set shape "circle"]
  create-planets 1 [ set color blue set size 1 set shape "circle" 
                     set xcor 12 set ycor 0 face sun 0 rt 90]
end
to go
  ask planets [ pen-down 
    fd velocity ;;; use a -10 to +10 slider here
    face sun 0
    fd .1
    rt 90 ]
end
```

*Created on 2020 December 23.*

[![Kakashi Public License Affirmed](https://github.com/13saints/licenses/blob/main/logos/KPLv1.0-affirmed-medium.png)](https://raw.githubusercontent.com/13saints/licenses/main/KPLv1.0.txt)