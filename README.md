# Dining Philosophers

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Implementation](#implementation)
- [Resources](#resources)

## Introduction

An implementation/solution to Dijkstra's dining philosophers problem for 42 School Lisboa. A table of philosophers each have a fork/chopstick between them and a bowl of spaghetti in the middle of the table. For a philosopher to eat, they must take both the fork to their left and the the fork to their right.

Each philosopher is a thread and each fork is protected by a mutex. Deadlocks, data races and philosopher deaths must be avoided wherever possible. There is no communication between philosophers but there is a monitor/waiter thread that can report if philosophers have died.

## Installation

Git clone the repository:

```shell
https://github.com/TimHopg/Dining-Philosophers.git
```

Run `make` from within the directory.

`make fclean` will remove program and object files.

## Usage

```shell
./philo [number_of_philos] [time_to_die] [time_to_eat] [time_to_sleep] [number_of_required_meals]
```

`number_of_philosophers` - Any number between `1` and `200`.

`time_to_die` - The time in milliseconds for a philosopher to die since the beginning of their last meal. Must be `> 60`.

`time_to_eat` - The time in milliseconds that it takes for each philosopher to finish their meal.

`time_to_sleep` - The time in milliseconds that each philosopher will sleep for before they can eat again.

`number_of_required_meals` is optional.

## Implementation

Because performance was paramount for this project and input limits were known, implementation was conducted entirely on the stack (excluding standard mutex implementation).

## Resources
