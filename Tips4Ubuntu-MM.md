Tips for Ubuntu-MM
==================

###`$`
Terminal မှ　User ၏　Command Prompt ကိုဆိုလိုခြင်းဖြစ်သည်။　Online မှ　Blog များ　Tutorial များတွင်　Command များကိုဖော်ပြရာ၌　ထည့်သွင်းဖော်ပြလေ့ရှိသည်။　သို့သော်　ထို　Command အား　ကူးယူ　အသုံးပြုရာတွင်　ထည့်သွင်းအသုံးပြုစရာမလိုပါ။　`$ sudo apt-get update` ဟုဖော်ပြထားပါက　`sudo apt-get update` ဆိုသော　command　 သာကူယူအသုံးပြုရန်လိုအပ်သည်။ 

`$` အား　စာလုံးတစ်ချို့နှင့်　ကပ်၍အသုံးပြုထားပါက　shell variable အဖြစ်　သတ်မှတ်ထားသည်ကို　ပြန်လည်ခေါ်ယူ　အသုံးပြုခြင်းဖြစ်သည်။　
```sh
$ var="Hello"
$ echo $var
Hello
```
အဆိုပါဥပမာရှိ　line တစ်ခုဆီ၏　ရှေ့တွင်တွေ့ရသော　`$` သည်　Command Prompt ကိုဆိုလိုခြင်းဖြစ်ပြီး　ဒုတိယ　line တွင်ပြထားသော　$var သည်　shell variable ကိုဆိုလိုခြင်းဖြစ်သည်။

---
###`#`
`$` ကဲသို့ပင်　Command များ၏ရှေ့တွင်　ေဖာ်ပြလေ့ရှိသည်။　`root　user` `super user` အနေဖြင့်　အသုံးပြုထားသော　Terminal ၏　Command Prompt ကိုဆိုလိုခြင်းဖြစ်သည်။　သာမန်　User Prompt `$` မှ Root User Prompt `#` သို့ ပြောင်းလိုပါက - `sudo -s` command ဖြင့်ပြောင်းနိုင်သည်။
```sh
$ sudo -s
[sudo] password for user: 
# 
```

---
###` ~/ `
သင်၏ `Home Directory` ကိုဆိုလိုခြင်းဖြစ်သည်။ တနည်းအားဖြင့် `/home/yourname` နှင့်တူညီသည်။

```sh
$ cd ~/
$ cd /home/yourname
```

---
###` ./ `
Terminal တွင် သင်ရောက်ရှိနေသော လက်ရှိ Directory ကို ဆိုလိုသည်။ Executable file များကို terminal မှတဆင့် run သောအခါတွင်အသုံးပြုလေ့ရှိသည်။ ဥပမာတွင်ပြထားသည်မှာ လက်ရှိ ရောက်ရှိနေသော Directory ထဲမှ script ဆိုသော Executable File ကို run လိုက်ခြင်းဖြစ်သည်။

```sh
$ ./script
```

---
###` . `
File သို့မဟုတ် Folder တို့၏ အမည်ရှေ့တွင် `.` ထည့်ပါက ထို File/Folder သည် File Manager ထဲတွင်သာမန်အားဖြင့် မြင်ရမည်မဟုတ်ပါ။ ထို File/Folder များအား File Manager တွင် မြင်နိုင်စေရန် `Control + H` Key အား နှိပ်၍ ဖော်နိုင်သည်။ အများအားဖြင့် System Configuration file များ folder များတွင်အသုံးပြုလေ့ရှိသည်။ User ၏ Home Directory `~/ ` ထဲတွင် `.local`, `.config` စသဖြင့်တွေ့နိုင်သည်။

---
###`sudo`
`root` တနည်းအားဖြင့် `super` user အနေဖြင့် command များ executable file များအား run သောအခါတွင်　သုံးသည်။ Windows တွင် Administrator အနေဖြင့် အသုံးပြုသည်နှင့် တူညီသည်။

---
###Command, Option and Parameter
Terminal တွင်း　အသုံးပြုသော　command များသည်　အများအားဖြင့်　လက်ရှိရောက်ရှိနေသော　Directory နှင့်　အတွင်းရှိ　File/Folder များတွင်သာ　သက်ရောက်သည်။　အထူးထပ်မံဖြည့်စွက်လိုက်သော　Options များ　Parameter များပေါ်မူတည်၍သာ　အပြောင်းအလဲများရှိသည်။　ဥပမာပြရလျှင်　`ls` command သည်　လက်ရှိရောက်ရှိနေသော　Directory ထဲမှ　File/Folder စာရင်းကို　ပြပေးသည်။　`ls /usr/share` ဟူ၍　parameter အနေဖြင့်　Directory Path `/usr/share` ကိုထည့်ပါက　ထို　Directory ထဲမှ　File/Folder များကိုပြပေးမည်ဖြစ်သည်။ 

Blog များ　Tutorial များတွင်ဖော်ပြထားသော　Linux Command များအား　ကူးယူအသုံးပြုရာတွင်　Error များ　တက်နိုင်ပါသည်။　အချို့ Command များမှာ မိမိ Install ပြုလုပ်မထားခြင်းကြောင့်　ဖြစ်နိုင်သလို　ကူယူရာတွင်　text format လွဲချော်ခြင်းကြောင့်လဲဖြစ်နိုင်ပါသည်။

Command များသည်　အများအားဖြင့်　အောက်ပါ　format အတိုင်းရှိတတ်ပါသည်။

```sh
$ wget -O skype-ubuntu-current_i386.deb http://www.skype.com/go/getskype-linux-beta-ubuntu-32
```
အဆိုပါစာကြောင်းတွင် `wget` သည် Internet ရှိ File များအား terminal မှတဆင့် Download ပြုလုပ်ရာတွင်သုံးသော command တစ်ခုဖြစ်သည်။　`-O` သည်　command ၏　Option ဖြစ်သည်။ Download ဆွဲလိုက်သော file အား နာမည်တစ်ခုဖြင့် ပြောင်းလဲစေလိုလျှင်သုံးပါသည်။ `-O` နောက်တွင်ရှိသော `skype-ubuntu-current_i386.deb` သည် ပြောင်းလဲလိုသော File နာမည်ဖြစ်ပြီး ၄င်း၏နောက်ရှိ `http://www.skype.com/go/getskype-linux-beta-ubuntu-32` သည် Download ပြုလုပ်မည့် File ရှိရာလမ်းကြောင်း (Link) ဖြစ်သည်။ ထို အစိတ်အပိုင်းတစ်ခုဆီ၏ ကြားတွင် Space ခြားထားသည်ကို သတိပြုရန်လိုအပ်သည်။

"wget```space```-O```space```skype-ubuntu-current_i386.deb```space```http://www.skype.com/go/getskype-linux-beta-ubuntu-32"

Command များအသုံးပြုရာတွင် `-`, `--`, နှင့် Space တို့ကို အထူးကရုပြုရမည်ဖြစ်ပြီး လွဲချော်နေပါက ထို Command အလုပ်လုပ်မည်မဟုတ်ပါ။

---