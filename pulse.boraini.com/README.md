# 🌸pulse.boraini.com🌸

In September 2024 I have bought myself a VPS to finally host some stuff without dealing with cloud deployments for once. I also host Minecraft servers. The server apps are accessed through a Nginx server. There is a Crafty Controller instance running which is used to start and stop Java-based applications, and also some system services. Here are all the endpoints that should be available:

- pulse.boraini.com - This should point to the server, and shouldn't be handled by anything other than the static Nginx website.
- pulse.boraini.com:8080 - Braillebot back-end - https://github.com/boraini/braillebot
- pulse.boraini.com:8443 - Crafty Controller is assumed to run here.
- crafty.boraini.com - The Crafty instance - Crafty Controller cannot work with a base path other than / therefore if we want to host other things on the server without an explicit port number, we need to add a proxy pass for Crafty.
