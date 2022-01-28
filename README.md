# Nexus

## About

The Kimerai (`kʲimeɾai`) project was started as a novel way to organize Discord bots. While current Discord bot implementations usually have every module under the same monolithic program, this is not necessarily the best way for a Discord bot to be created.

Discord bots are often projects taken on by novices, and as a result, many online resources often don't cover certain things that could be highly beneficial to certain types of bots. However, I know nothing about the intricacies of bots; Kimerai goes off the beaten path solely for the sake of exploration and curiosity.

As stated before, the Kimerai project was started as a novel way to organize Discord bots. Kimerai attempts to decouple frontend and backend code. Frontends are split into `scylla` and `charybdis`, the projects for the Discord bot frontend and the website frontend respectively. Backends are split into "modules" which are analogous to what some Discord libraries call "cogs".

This modularity is Kimerai's greatest strength. The decoupling frontend and backend forces an architecture which is test-friendly. Furthermore, splitting up different components of the backend allows for them to be dynamically horizontally scaled, independent of each other. This modularity also allows for selective deployment: you only deploy the modules that you want. I guess it's also cool that [Docker recommends this approach](https://docs.docker.com/config/containers/multi-service_container/).

## Getting started

The recommended way to deploy Kimerai is by using the Helm chart provided in this respository. You're probably a masochist if you want to run it some other way.

## Contributing

If you have a suggestion that would make this better, please fork the repo and create a pull request. Or open an issue with the tag "enhancement". Up to you.

## License

Kimerai is distributed under the MIT License. See `LICENSE.txt` for more information.
