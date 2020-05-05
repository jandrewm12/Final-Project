# INFOTC 1000 Final Project
## Page 3
![tree banner](https://www.ppt-backgrounds.net/uploads/tree-banner-quality-image.jpeg)

I like to listen to music as well! I prefer to listen to rock and metal bands.

My **favorite** bands are:
- *Motionless in White*
- *My Chemical Romance*
- *Wage War*
- *The Amity Affliction*
- and many more!

However! I like to listen to all sorts of other kinds of music as well! **Especially** classical and instrumental music!
Joe Hisaishi is my favorite composer, most well-known for composing the music we hear in Studio Ghibli movies. **[Beautiful stuff](https://www.youtube.com/watch?v=TK1Ij_-mank).**

![Joe Hisaishi](joehisaishi.jpg)

Once again, here's another block of code from INFOTC 1040:
```
import math

#constants
GALLON = 350
LABOR_COST = 62.25
LABOR_HOURS_PER_GAL = 6

def get_float_input(prompt):
    #get values from user
    while(True):
        try:
            float_value = float(input(prompt))
            if float_value < 0:
                print("Please enter a positive value")
                continue
        except ValueError:
            print("Please enter a number.")
        else:
            break
    return float_value

def main():
    while(True):

        #get square feet from user
        wall_space = get_float_input("How many square feet are being painted? ")

        #get price per gal from user
        price = get_float_input("How much does paint cost per gallon (in $)? ")

        #get gallons required
        gallons_required = (math.ceil(wall_space/GALLON))

        #calculate hours of required labor
        labor_hours = (wall_space/GALLON)*LABOR_HOURS_PER_GAL

        #calculate total paint cost
        paint_cost = gallons_required * price

        #calculate labor charges
        labor_charges = labor_hours * LABOR_COST

        #total
        total = paint_cost + labor_charges

        #output information
        print("Gallons of Paint Required: " + str(gallons_required))
        print("Hours of Required Labor: " + str(round(labor_hours, 1)))
        print("Total Cost of Paint: $" + str(round(paint_cost, 2)))
        print("Total Cost of Labor: $" + str(round(labor_charges, 2)))
        print("Total Cost: $" + str(round(total, 2)))

        #ask to repeat
        do_again = input("Press 'y' to do again. Press any other key to end. ")

        if do_again != 'y':
            break

#function
main()
```

That program estimates the price of a paint job!

---

Navigate between pages:
- [Page One](page1.md)
- [Page Two](page2.md)
- Page Three
- [Page Four](page4.md)
- [Page Five](page5.md)
