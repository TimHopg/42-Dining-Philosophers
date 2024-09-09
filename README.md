# Dining Philosophers

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Resources](#resources)

## Installation
Git clone the repository:
```shell
https://github.com/TimHopg/Dining-Philosophers.git
```

Run `make` from within the directory.
`make fclean` will remove program and object files.

## Usage
```shell
./philo number_of_philos time_to_die time_to_eat time_to_sleep [number_of_required_meals]
```
`number_of_philosophers` - Any number between `1` and `200`.

`time_to_die` - The time in milliseconds for a philosopher to die since the beginning of their last meal. Must be `< 60`.

`time_to_eat` - The time in milliseconds that it takes for each philosopher to finish their meal.

`time_to_sleep` - The time in milliseconds that each philosopher will sleep for before they can eat again.

`number_of_required_meals` is optional.

## Resources