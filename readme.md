Battle Robots
=============

![FLUX.1 dev a small wheeled robot battling a small tracked robot using a large hammer. cute. plain white background.](https://github.com/user-attachments/assets/c908910f-2950-48f1-916e-acf093aec98f)


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

