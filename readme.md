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

Task
----

Handout code is provided in [bot.py](bot.py). It includes a number of failing test for new features. These features should be added to make the tests pass:

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

Optional Task
-------------

Once the classes are implemented, bots will battle in a simulated arena. The `MyBot` simply moves randomly. Adjust the `MyBot` class so that it defeats the `AngryBot` that is a `SuperBot` constantly attacking.
