# My commercial programming story

My programming journey started rather early, at the age of 10 (2009). And only two years later (yes, at the age of 12) I started applying my nascent programming skills and knowledge commercially. I lived with grandparents who had a pension that was comparatively high but low in absolute numbers, so I had to work part-time to enjoy [tarkhun](https://en.wikipedia.org/wiki/Tarkhuna_(drink)), [baikal](https://en.wikipedia.org/wiki/Baikal_(drink)), and pizza or simply even be able to buy water so that I could play soccer with my friends without suffering from thirst.

Legally, working even part-time in Russia is possible only at the age of 14, so I had to work on [Onionland](https://en.wiktionary.org/wiki/Onionland) forums via Tor to circumvent the legal barrier that I consider unfair up to this day. My tools at the time were [Cheat Engine](https://en.wikipedia.org/wiki/Cheat_Engine) for dynamic analysis, custom-patched [IDA Pro](https://en.wikipedia.org/wiki/Interactive_Disassembler) for static analysis, and a [Dr.Web](https://en.wikipedia.org/wiki/Dr.Web)-based unpacker for cracking then-state-of-the-art Armadillo Software Protection System. *I deliberately never wrote, distributed, or in any way participated in the development of any malware.*

In 2013, I crated an account on no-longer-operational [фриланс.рф](фриланс.рф) where I started creating simple static landing pages with HTML, CSS, and a little bit of JavaScript (after approximately a half of a year of learning). Even at that point I did not have a GitHub or moreover GitLab account.

In 2015, I received a request from my friend employed by [Advance Roleplay](https://www.adv-rp.com/about_us/) project to write a script that would help him and his colleagues perform their administrator duties easier and more effectively. He knew that admins on other projects used scripts written in C++-like [AutoHotkey](https://en.wikipedia.org/wiki/AutoHotkey) programming language. Fast-forward 2 years and in 2017 I become the top-2 on-demand AutoHotkey scripter in Russia due to [silly-yet-technical humour](https://vk.com/deemakid?w=wall82826648_1044) (that appealed to many of my peers) and close collaboration with my clients.

![screenshot](https://i.imgur.com/WMp9aAv.png)

*[The post](https://vk.com/wall82826648_1150) reads ["For feedback"](https://translate.google.com/?sl=ru&tl=en&text=%D0%B4%D0%BB%D1%8F%20%D0%BE%D1%82%D0%B7%D1%8B%D0%B2%D0%BE%D0%B2%20%D0%BE%20%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%B5&op=translate&hl=en)*

* Script that puts the [hovered](https://www.merriam-webster.com/dictionary/hover) player on the wanted list, notifies everyone in the police department about that, and informs the staff about the location of the crime scene. Client: [Захар Алексеевич](https://vk.com/qw2143).

> "[The author] completed the task in a short time, excellent work. [I] recommend.".
> 
> Original: ["Сделал то, что требуется в короткие сроки, работа отличная. Советую обращаться."](https://vk.com/deemakid?w=wall82826648_1150_r1152).
>
> Google Translate's take: ["He did what was required in a short time, the work is excellent. I advise you to apply."](https://translate.google.com/?sl=ru&tl=en&text=%D0%A1%D0%B4%D0%B5%D0%BB%D0%B0%D0%BB%20%D1%82%D0%BE%2C%20%D1%87%D1%82%D0%BE%20%D1%82%D1%80%D0%B5%D0%B1%D1%83%D0%B5%D1%82%D1%81%D1%8F%20%D0%B2%20%D0%BA%D0%BE%D1%80%D0%BE%D1%82%D0%BA%D0%B8%D0%B5%20%D1%81%D1%80%D0%BE%D0%BA%D0%B8%2C%20%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%B0%20%D0%BE%D1%82%D0%BB%D0%B8%D1%87%D0%BD%D0%B0%D1%8F.%20%D0%A1%D0%BE%D0%B2%D0%B5%D1%82%D1%83%D1%8E%20%D0%BE%D0%B1%D1%80%D0%B0%D1%89%D0%B0%D1%82%D1%8C%D1%81%D1%8F.&op=translate&hl=en).

* Secure Admin Log-in software package (written before the post). Client: [Дмитрий Кот](https://vk.com/kowka228). This solution consists of several components:
  - Admin ID Generator. The one-time executable that obtained the serial number of the hard drive, and requested the server to finalize giving the admin rights to the account on the active SAMP launcher. In the process, it also assigned the admin a unique ID, hence the name. It also had a simplistic GUI that displayed such information as IP, encrypted serial number of the hard-drive, and the nickname of the active SAMP account. Upon competion, the application displayed a congratulatory window and overwrote the clipboard with the new admin ID, which the new administrator was supposed to keep secret. Since the access to the Admin ID Generator was supposed to be provided via one-time link and only over a screen-sharing session on Skype and the application was fairly useless for anyone without the pre-authorization, the Admin ID Generator never received its own builder.
  - Minimal PHP & MySQL server implementing the necessary routing and handlers, including those for keeping the track of the admin data records, as well as those for providing REST API for verification of one-time passwords-hashes generated based on the serial numbers of the hard drives and time (for up to 3 secs difference).
  - Secure Admin Log-in application builder. This builder was supposed to build binary-wise distinct yet functionally equivalent applications for each new admin so that the leaks of the applications were identifiable. Functionally, any of these applications would notify the server about being ran on a particular hardware (serial number of the hard drive) and on a particular IP so that the server could instantly remove the admin rights of the suspected admin if their admin ID is compomised and so that the admin could log-in with dynamically-generated passwords hassle-free.
  
  > Found in the conversation in VK (Вконтакте).

* Assistance with Google Authentication for regular users via [PHPGangsta/GoogleAuthenticator](https://github.com/PHPGangsta/GoogleAuthenticator). Client: [Дмитрий Кот](https://vk.com/kowka228).

> [The author] helped with Google Authenticator Web API in short time. I'm very grateful, thanks.
> 
> Original: ["Помог с Web API Google Authenticator за короткое время. I'm very blagodaren, thanks."](https://vk.com/deemakid?w=wall82826648_1150_r1154).
>
> Google Translate's take: ["Helped with Google Authenticator Web API in a short time. I'm very grateful, thanks."](https://translate.google.com/?hl=en&sl=ru&tl=en&text=%D0%9F%D0%BE%D0%BC%D0%BE%D0%B3%20%D1%81%20Web%20API%20Google%20Authenticator%20%D0%B7%D0%B0%20%D0%BA%D0%BE%D1%80%D0%BE%D1%82%D0%BA%D0%BE%D0%B5%20%D0%B2%D1%80%D0%B5%D0%BC%D1%8F.%20I%27m%20very%20blagodaren%2C%20thanks.&op=translate).

