
Slack SimpleBot
===============

Slack bot engine for realtime protocol.


Examples
--------

::

    from slack_simplebot import SlackRtm
    from slacker import Slack

    client = Slack()
    rtm = SlackRtm.from_slacker(client, debug=True)

    @rtm.command('hello')
    def say_hello(event, *args):
        rtm.send_mesage(...)
