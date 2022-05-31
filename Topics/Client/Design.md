
# Design

<br>
<br>

<div align = center>

[![Design]](#)

</div>

<br>
<br>

The client is written using **[Deno]** and consists <br>
of the major parts seen in the above graphic.

<br>
<br>

## WebSocket

The websocket is used to communicate <br>
with the interface for a variety of things.

<br>

### Uses

- Requesting the client to synchronize the machine

- Requesting the client to open the project's page.

- Requesting spice / recipe data from the client

- Writing spice / recipe data to the client

<br>
<br>

## WebServer

The webserver locally hosts interface files as a website.

<br>
<br>

## WebView

The webview is a responsible for serving the browser <br>
windows that acts as the 'physical' program window.

<br>
<br>

## Serial

The serial code interact with the `libserial` library <br>
to send / receive data from the connected machine.

<br>


<!----------------------------------------------------------------------------->

[Design]: ../../Resources/Client/Design.png
[Deno]: https://deno.land/
