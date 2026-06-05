
<h1 align="center">
    <samp>တယ်လီဂရမ် ချန်နယ် မိတ္တူကူးယူရေး</samp>
</h1>

<p align="center">
    တယ်လီဂရမ် ချန်နယ်တစ်ခုမှ အကြောင်းအရာအားလုံးကို မိတ္တူကူးယူရန် script တစ်ခု။ <br />
    သတ်မှတ်ထားသော တယ်လီဂရမ် ချန်နယ်တစ်ခုမှ စာသားများ၊ ရုပ်ပုံများနှင့် လင့်ခ်များ အပါအဝင် မက်ဆေ့ချ်အားလုံးကို ရယူသိမ်းဆည်းပေးပြီး အရန်သိမ်းဆည်းမှုနှင့် ဝင်ရောက်ကြည့်ရှုရာတွင် လွယ်ကူစေသည်။
</p>

<p align="center">
    <img alt="GitHub License" src="https://img.shields.io/github/license/Warnigo/telegram-chanal-copy?style=flat&label=license&labelColor=%23ffffff&color=%23454545">
</p>

---

## ✨ အင်္ဂါရပ်များ

- 📋 မည်သည့် **တယ်လီဂရမ် ချန်နယ် သို့မဟုတ် အုပ်စု** ကိုမဆို မိတ္တူကူးယူနိုင် (အများပြည်သူနှင့် သီးသန့် နှစ်မျိုးလုံး အလုပ်လုပ်)။
- 🔄 အကြောင်းအရာများကို မိတ္တူကူးယူရန် သင်သည် **ရင်းမြစ် ချန်နယ် သို့မဟုတ် အုပ်စုတွင် အဖွဲ့ဝင်ဖြစ်ရပါမည်**။
- 🛠 စာသား၊ ရုပ်ပုံများ၊ PDF နှင့် ဗီဒီယိုများကို အလိုအလျောက် ကိုင်တွယ်ပြီး ထိရောက်စွာ အရန်သိမ်းပေးသည်။

---

### 📂 ဤ repository ကို clone လုပ်ရန်

```sh
git clone https://github.com/Warnigo/telegram-chanal-copy.git

cd telegram-chanal-copy
```

## 🛠 ပြင်ဆင်သတ်မှတ်ချက်

### 1. အသုံးမပြုမီ [config.py](./config.py) ဖိုင်ကို တည်းဖြတ်ပါ

- `API_ID` နှင့် `API_HASH` - [my.telegram.org](http://my.telegram.org/) မှ ရယူပါ။
- `PHONE_NUMBER` - နိုင်ငံကုဒ်အပါအဝင် ဖုန်းနံပါတ် ထည့်ပါ (ဥပမာ +998901234567)။
- `NAME` - မိမိနှစ်သက်ရာ အမည်တစ်ခု ပေးပါ။
- `SOURCE_CHAT_ID` နှင့် `DESTINATION_CHAT_ID` - [@username_idbot](https://telegram.dog/username_idbot) မှ ရယူပါ။

#### `config.py` နမူနာ:

```python
class Config:
    API_ID = "12345678"            # သင်၏ API ID
    API_HASH = "your_api_hash"     # သင်၏ API Hash
    PHONE_NUMBER = "+998901234567" # သင်၏ ဖုန်းနံပါတ် (နိုင်ငံကုဒ်အပါအဝင်)
    NAME = "telegram-channel"      # သင်ရွေးချယ်သော အမည်
    SOURCE_CHAT_ID = -1001234567890 # ရင်းမြစ် ချန်နယ်/အုပ်စု ID
    DESTINATION_CHAT_ID = -1009876543210 # ဦးတည်ရာ ချန်နယ်/အုပ်စု ID
```

>[!NOTE]
> နေရာလွတ်များတွင် သင်၏ အထောက်အထားစစ်မှန်သော အချက်အလက်များကို အစားထိုးထည့်သွင်းရန် သေချာပါစေ။

### 2. config.py ဖိုင် ဖန်တီးပါ

မရှိသေးပါက ပြင်ဆင်သတ်မှတ်မှုဖိုင် ဖန်တီးပါ:

```bash
touch config.py
```

## 🐍 Virtual Environment ပြင်ဆင်သတ်မှတ်ခြင်း

အကြံပြုလိုသည်မှာ dependencies ပဋိပက္ခများကိုရှောင်ရှားရန် virtual environment ကိုသုံးစွဲခြင်းဖြစ်သည်။

### 1. Virtual Environment တစ်ခု ဖန်တီးပါ
- #### Windows

```sh
python -m venv myenv
```

- #### macOS နှင့် Linux

```sh
python3 -m venv myenv
```

### Virtual Environment ကို အသက်သွင်းရန်

- #### Windows

```powershell
.\myenv\Scripts\activate
```

- #### macOS နှင့် Linux

```bash
source myenv/bin/activate
```

> [!NOTE]
> Virtual environment ကို မည်သည့်အချိန်တွင်မဆို ပိတ်ရန် အောက်ပါ command ကို ရိုက်ထည့်ပါ:

```bash
deactivate
```

## 📦 Dependencies များ ထည့်သွင်းခြင်း

ဤ script သည် Telegram နှင့် အလုပ်လုပ်ရန် Telethon library ကို အသုံးပြုသည်။

### [telethon](https://pypi.org/project/Telethon/) ကို ထည့်သွင်းရန်

- #### Windows

```powershell
pip install telethon
```

- #### macOS နှင့် Linux

```bash
pip3 install telethon
```

## 🚀 Script ကို run ခြင်း

### အကြောင်းအရာများ စတင်ကူးယူရန်:

- #### Windows

```powershell
python bot.py
```

- #### macOS နှင့် Linux

```bash
python3 bot.py
```

## 📋 အသုံးပြုမှု လမ်းညွှန်ချက်များ
Script ကို run သည့်အခါ ရင်းမြစ်ချန်နယ်မှ မက်ဆေ့ချ်အသစ်များကိုသာ ကူးယူမလား၊ သို့မဟုတ် မက်ဆေ့ချ်အားလုံးကို ပြန်လည်ပို့မလားဟု မေးမြန်းလိမ့်မည်။

- ရင်းမြစ်ချန်နယ်မှ ဦးတည်ရာသို့ မက်ဆေ့ချ်အသစ်များကိုသာ ကူးယူရန် `y` ကို ရိုက်ထည့်ပါ။
- ရင်းမြစ်မှ ဦးတည်ရာသို့ မက်ဆေ့ချ်အားလုံးကို ပြန်လည်ကူးယူရန် `n` ကို ရိုက်ထည့်ပါ။

>[!NOTE]
> အကယ်၍ သင်သည် script ကို ရပ်တန့်လိုက်ပြီး ပြန်စပါက သင်ရပ်တန့်ခဲ့သည့်နေရာမှ ဆက်လုပ်ရန် သို့မဟုတ် အစမှ ပြန်စရန် ရွေးချယ်နိုင်သည်။

## 🛠 ပြဿနာဖြေရှင်းခြင်း
- Script ကို run မလုပ်မီ ရင်းမြစ်နှင့် ဦးတည်ရာ ချန်နယ်/အုပ်စု နှစ်ခုလုံးတွင် သင်အဖွဲ့ဝင်ဖြစ်ကြောင်း သေချာပါစေ။
- အထောက်အထားစစ်ဆင်ရေးအမှားများတွေ့ပါက သင်၏ API အထောက်အထားများကို ထပ်မံစစ်ဆေးပါ။
Script မမျှော်လင့်ဘဲ ရပ်သွားပါက ပြန်လည် run နိုင်ပါသည်။ မည်သည့်အကြောင်းအရာကို ကူးယူမည်ကို ထိန်းချုပ်ရန် y/n prompt ကို အသုံးပြုပါ။

## ❤️ အကူအညီ
ဤပရောဂျက်သည် အသုံးဝင်သည်ဟု သင်ထင်ပါက repository ကို ⭐️ star ပေးခြင်းဖြင့် သင်၏အားပေးမှုကို ပြသပါ။

<p align="center"> <samp>Warnigo မှ ❤️ ဖြင့် ပြုလုပ်ထားသည်</samp> </p>

