# Brick Breaker

**Brick Breaker** is a Breakout-style game built with **C#** and **MonoGame**.
Use your racket to keep the ball in play and clear every brick on the board.

<img src="./images/cover/cover.png" width="450" />

## Gameplay

- Move the racket left and right to bounce the ball.
- Break all bricks to win the level.
- Do not let the ball fall below the racket.

### Controls

- Left Arrow: Move left
- Right Arrow: Move right

## Game Objects

<table border="1" cellspacing="0">
 <tr>
  <th>Racket</th>
  <th>Ball</th>
  <th>Brick</th>
 </tr>
 <tr>
  <td>
   <img src="./images/player/racket.png" width="150" />
  </td>
  <td>
   <img src="./images/objects/ball.png" width="150" />
  </td>
  <td>
   <img src="./images/objects/block.png" width="150" />
  </td>
 </tr>
</table>

## Gallery

<table border="1" cellspacing="0">
 <tr>
  <td>
   <img src="./images/gameplay/gameplay_1.png" width="350" />
  </td>
  <td>
   <img src="./images/gameplay/gameplay_2.png" width="350" />
  </td>
  <td>
   <img src="./images/gameplay/gameplay_3.png" width="350" />
  </td>
 </tr>
 <tr>
  <td>
   <img src="./images/gameplay/gameplay_4.png" width="350" />
  </td>
  <td>
   <img src="./images/gameplay/gameplay_5.png" width="350" />
  </td>
 </tr>
</table>

## Installation

### Prerequisites

- Windows OS
- .NET 10 SDK (preview or newer)
- Git

### 1. Clone the repository

```bash
git clone https://github.com/idanbachar/brick-breaker.git
cd brick-breaker
```

### 2. Restore dependencies

```bash
dotnet restore "Brick Breaker/Brick Breaker.sln"
```

### 3. Build the game

```bash
dotnet build "Brick Breaker/Brick Breaker.sln"
```

### 4. Run the game

```bash
dotnet run --project "Brick Breaker/Brick Breaker.csproj"
```

## Project Stack

- C#
- MonoGame `3.8.4.1`
- DesktopGL platform

## License

Copyright © 2026 Idan Bachar. All rights reserved.

This project and its code are proprietary. No part of this software may be copied,
distributed, or modified without the express written permission of the owner.