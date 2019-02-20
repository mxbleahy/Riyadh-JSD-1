## Promise Foods Exercise

Time to use your freshly honed Promise skills to to order some food from Promise Burger. For this exercises you will use some code that is already imported into hw.js called kitchen. The methods on the kitchen object all return a Promise, so you will need to use the two methods we learned about in class to respond to the Promise.

You only need to edit code in hw.js

### Look at the Menu

Promise Foods has a method called `.readMenu`. Call this method and `console.log` the data that returns.

### Order Some Food

For this task, you will use the method .order to order the cheapest burger on the menu. The order method has one argument, the name of the burger you would like to order. Once the promise has been resolved, console.log "Man that burger sure was tasty!".

Try and use the same method to order a quesadilla. Since Promise Burger only serves burgers, this will throw an error. Make sure that your Promise can be dealt with when it is rejected.

### Add A Burger To The Menu

Promise Foods also has a method called addToMenu. This method has one argument, which expects an object with a name, price, and description. Use this method to add this burger to the menu. Add a method to console.log the response once the promise is resolved!
```
{
  "name": "TRIPLE CORONARY BYPASS",
  "price": 28.95,
  "description": ` It becomes difficult to even describe this, the most preposterous of our Bypass Burgers. All you really need to know is that we use three burger patties, three fried eggs, fourteen slices of American cheese, and ten slices of bacon, all packed between two grilled cheese sandwiches. Figuring out how to add condiments is completely up to you. It’s served in a big bowl of french fries and tater tots covered, in lots of our Cheesy-Cheese Goo. Enjoy!`
}
```

Validate that the new item has been added to the menu by calling readMenu again. We only want to call readMenu after we get a response that is successful. Remember that we can `.then` calls together the same way that we can chain jQuery methods.

### Stretch Goals

Let's be honest, people only go to Promise Foods when they are showing out-of-towners around. You old college roommates are all visiting Atlanta and want to try out this place. They already know what they want to eat!
```
const customers = [
  {
    name: "Josie",
    order: "HOLY GUACAMOLE"
  }, {
    name: "Chris",
    order: "BIG BLUE BUFFALO"
  }, {
    name: "John",
    order: "BLUE 'SHROOM",
  }, {
    name: "Katelyn",
    order: "FAT ELVIS"
  }
]
```

Loop through each customer and use the .order function on each object within the array. Then console.log All Food Delivered when ALL of the promises have been resolved. This will require you to use the Promise.all method we haven't covered in class. See if you can find it on the docs page.

[Promises - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)

Hint Look at the Promise methods on the left hand side of the page.

### Submission

Get as far as you can with these exercises before the due date.

- push to github and send a pull request.
- Add a comfort score between 1-5 on how confident you feel about understanding promises.
- Write 2-3 sentences on either a breakthrough you had while building out promises or a problem that you couldn't debug and would like additional support on.