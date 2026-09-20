<div align="center">

# Discord Username Checker

**I have been gate keeping this project for years now, it's time I release it.**


</div>

## Features

- **Multi-Proxy support** - Works with any proxy format with validation  
- **Generation** - Creates usernames by length (3-6 chars)
- **Saves Results** - Saves your hits by date
- **Live progress** - Shows progress as it runs

## Usage

1. Run `discord-username-checker.exe`
2. Add your proxies to `proxies.txt` (this gets created on first run)
3. Pick how you want to check
4. the rest is automated

---

## Setup

### Proxies (You need these)

Add them to `proxies.txt` - one per line:

```ini
http://user:pass@proxy.com:8080
socks5://proxy2.com:1080
user:pass@proxy.com:8080
proxy.com:8080
```

### Usernames (Optional)

Add specific usernames to check to `usernames.txt`:

```ini
ieatrocks
wombo
scarlett_johansson
```

---

## How It Works

**[1] Check from file** - Checks your username list  
**[2] Generate by length** - Creates random usernames and checks them  
**[3] Settings** - See current settings  
**[4] Exit** - Close the app  

## Your Results

Everything gets saved in `hits/`:

```ini
hits/10-24-2025/available.txt
```

What you'll see:

```ini
username1             │ 10/24/2025 16:07:43
username2             │ 10/24/2025 16:08:57
username3             │ 10/24/2025 16:08:09
```

## Settings

Edit `config.json` if you want to change anything:

```json
{
  "threads": 10,
  "max_generate": 15,
  "min_length": 3,
  "max_length": 6
}
```

---

## Note

- **Needs proxies** - Won't work without them
- **This only checks** - it does not auto-register them
> **Need proxies?** Get some from [proxies.rip](https://proxies.rip/). they work well

## License

[MIT](LICENSE) © [YourPOVV](https://github.com/yourpovv)

