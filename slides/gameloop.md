# Game loop


Note: it's the heart of the game

--

Almost every game uses a game loop.<br>This is probably the most used game programming pattern.

--

> A **game loop** runs continuously during gameplay.
> Each turn of the loop, it **processes user input** without blocking, **updates the game state**, and **renders the game**.
> It tracks the passage of time to **control the rate of gameplay**.

<div class="attribution">[Robert Nystrom: Game Programming Patterns](http://gameprogrammingpatterns.com/game-loop.html)</div>

--

<img data-src="images/game-loop-simple.png" class="stretch">

<div class="attribution">Photo: [Robert Nystrom: Game Programming Patterns](http://gameprogrammingpatterns.com/game-loop.html)</div>

--

```C
while (true)
{
    processInput();
    update();
    render();
}
```

--

```C
while( user doesn't exit )
    check for user input
    run AI
    move enemies
    resolve collisions
    draw graphics
    play sounds
end while
```

--

# JavaScript Example

```JavaScript
(function loop() {
    // start over in the next frame
    requestAnimationFrame(loop);

    // process user input
    // update
    // draw    
    // play sounds
}());
```

--

# Game loops are<br>not just for games

--

```C
while (softwareIsRunning) {
    processInputs();
    updateBusinessObjects();
    generateOutput();
}
```

--

### Idea: Real-time advertising

In every "frame":
- we process clicks on ads
    - each click costs some money for the advertiser
    - each click earns some money for the publisher
- we update the earnings/expenses
- we put the newly computed values into a database

--

### Idea: Real-time advertising

```C
while(true) {
    processClicksOnAdsSinceLastFrame();
    
    updateEarnings();
    updateExpenses();

    putChangedValuesToDB();
}
```
