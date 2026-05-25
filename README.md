import requests

webhook_url = "https://discord.com/api/webhooks/1508253719878303795/Ir4MjRXI2s_d8skPmX9u06m24WlHHeVKBGGTH8QRqdm3dxSDdcfsXnQhlnFyxLCKQxEm"

embed = {
    "title": "📜 Discord Community Rules",
    "description": (
        "Welcome to our Melody Family community!\n"
        "Different families, one community — let’s keep this server fun, respectful, and welcoming for everyone."
    ),
    "color": 15277667,
    "fields": [
        {
            "name": "1. Respect Everyone",
            "value": "Friendly banter is okay, personal attacks and toxic behavior are not.",
            "inline": False
        },
        {
            "name": "2. Different Families, Same Community",
            "value": "Rivalries stay inside the game. Outside the game, we treat each other like teammates.",
            "inline": False
        },
        {
            "name": "3. No Drama & Unnecessary Fights",
            "value": "Solve issues calmly or ask moderators for help.",
            "inline": False
        },
        {
            "name": "4. Keep Chats Clean & Comfortable",
            "value": "Avoid spam, offensive content, and anything that ruins the vibe.",
            "inline": False
        },
        {
            "name": "5. Help New and Returning Players",
            "value": "A small guide or kind answer can make someone stay in the community.",
            "inline": False
        },
        {
            "name": "6. Use Channels Properly",
            "value": "Keep topics in the correct channels to avoid clutter.",
            "inline": False
        },
        {
            "name": "7. Have Fun & Make Memories",
            "value": "Events, grinding, raids, or random talks — enjoy the community together.",
            "inline": False
        }
    ],
    "footer": {
        "text": "Melody Family"
    }
}

data = {
    "username": "Melody Rules",
    "embeds": [embed]
}

requests.post(webhook_url, json=data)