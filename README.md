# base16
import requests

API_KEY = "YOUR_BASESCAN_API_KEY"

url = f"https://api.basescan.org/api?module=stats&action=addresscount&apikey={API_KEY}"

response = requests.get(url)
data = response.json()

print(data)
