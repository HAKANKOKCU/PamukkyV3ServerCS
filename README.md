# Pamukky V3 Server C#
https://pamukky.netlify.app/v3

Rewritten version of [PamukkyV3ServerNode](https://github.com/HAKANKOKCU/PamukkyV3ServerNode). Why? Javascript kinda sucks and the code was messy.

In this rewrite, I made almost everything classes. So it should be better.
# How to run?
## Normal
- Install dotnet
- cd to the folder which has .csproj
- `dotnet run [-- "port" "port for https"]` ( [] is optional, port is a number)

## Docker
- cd to the folder which has .csproj
- Build the docker: `docker build -t pamukky -f Dockerfile .`
- Run the docker: `docker run -p 4268:4268 pamukky`

# Status
I think it's usable, but expect some bugs.
Few functions are still partial and not implemented.

# Notes
* Https is a todo. For now you can forward the requests to https.
* C#'s HTTP listener needs firewall rules.
* Force quitting will not save chats unless autosave saved them.
