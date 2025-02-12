Battle Robots
=============

- Create a ZapBot class that implements a new `get_attacks` method. This should apply 1 damage to all bots adjacent to us.

```
⚡⚡⚡
⚡🤖⚡
⚡⚡⚡
```

- Create a SmashBot class that implements a new `get_attacks` method. This should apply 5 damage to the bot on the space directly in front of us.

```
🔨
🤖

🤖🔨
```

- Create a FlameBot class that implements a new `get_attacks` method. This should apply 3 damage to any bots up to 3 spaces directly in front of us.

```
🔥
🔥
🔥
🤖

🤖🔥🔥🔥
```

- Create a SuperBot class that inherits from the 3 others and performs all three attacks simultaneously.

```
⚡⚡⚡
⚡🤖🔨🔥🔥🔥
⚡⚡⚡
```

