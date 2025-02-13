Battle Robots
=============

A lab to explore multiple inheritance in Python.

![FLUX.1 dev a small wheeled robot battling a small tracked robot using a large hammer. cute. plain white background.](https://github.com/user-attachments/assets/4a8b1445-0e2b-4b33-ad16-e0cb1f330ef1)

Learning Objectives
-------------------

After completing this lab, students will be able to:

- Navigate inheritance hierachies
- Create classes that inherit from one another
- Leverage multiple inheritance

Tasks
-----

Handout code is provided in [bot.py](bot.py). It includes a number of failing tests for new features. These features should be added to make the tests pass:

- Our bots need to be able to `Move` and `Attack`. Create a `Move` class the extends `Action`. `Move` should have a single attribute, `direction` that can be set as the single parameter of the constructor.

- Create an `Attack` class that also extends `Action`. An attack represents damage to be applied at a particular positions. Attacks have `x`, `y`, and `damage` attributes that can be set in that order using the constructor.

- Create a `ZapBot` class that implements a new `get_attacks` method. This should apply 1 damage to all bots adjacent to us:

```
⚡⚡⚡
⚡🤖⚡
⚡⚡⚡
```

- Create a `SmashBot` class that implements a new `get_attacks` method. This should apply 5 damage to the bot on the space directly in front of us:

```
🔨
🤖

🤖🔨
```

- Create a `FlameBot` class that implements a new `get_attacks` method. This should apply 3 damage to any bots up to 3 spaces directly in front of us:

```
🔥
🔥
🔥
🤖

🤖🔥🔥🔥
```

- Create a `SuperBot` class that inherits from `ZapBot`, `SmashBot`, and `FlameBot` that performs all three attacks simultaneously:

```
⚡⚡⚡
⚡🤖🔨🔥🔥
⚡⚡⚡
```

Coordinates
-----------

Bots operate on a [Cartesian coordinate system](https://en.wikipedia.org/wiki/Cartesian_coordinate_system). The top left of our simulated world is at 0,0. All valid positions are positive. This is the same system used in many other tools, such as the [HTML Canvas element](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes).

![Canvas coordinate system](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes/canvas_default_grid.png)


Optional Task
-------------

Once the classes are implemented, bots will battle in a simulated arena. The `MyBot` simply moves randomly. Adjust the `MyBot` class so that it defeats the `AngryBot` that is a `SuperBot` constantly attacking.
