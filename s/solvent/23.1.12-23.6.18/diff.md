# Comparing `tmp/solvent-23.1.12.tar.gz` & `tmp/solvent-23.6.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solvent-23.1.12.tar", max compression
+gzip compressed data, was "solvent-23.6.18.tar", max compression
```

## Comparing `solvent-23.1.12.tar` & `solvent-23.6.18.tar`

### file list

```diff
@@ -1,117 +1,116 @@
--rw-r--r--   0        0        0      885 2023-01-13 00:16:25.629096 solvent-23.1.12/pyproject.toml
--rw-r--r--   0        0        0       76 2022-06-12 15:47:00.426483 solvent-23.1.12/solvent/__init__.py
--rw-r--r--   0        0        0       60 2021-03-28 14:36:20.977593 solvent-23.1.12/solvent/__main__.py
--rw-r--r--   0        0        0     2472 2022-08-28 23:22:06.463218 solvent-23.1.12/solvent/cli.py
--rw-r--r--   0        0        0      811 2022-08-28 23:50:25.633733 solvent-23.1.12/solvent/gui.py
--rw-r--r--   0        0        0     1926 2022-08-27 18:08:12.941410 solvent-23.1.12/solvent/scripts/__init__.py
--rw-r--r--   0        0        0     7611 2022-12-04 22:08:27.537912 solvent-23.1.12/solvent/scripts/gop.py
--rw-r--r--   0        0        0     1839 2022-10-11 12:18:46.768984 solvent-23.1.12/solvent/scripts/lindell.py
--rw-r--r--   0        0        0     5613 2022-12-17 05:41:24.054728 solvent-23.1.12/solvent/scripts/misc.py
--rw-r--r--   0        0        0      701 2020-12-31 22:26:05.898046 solvent-23.1.12/solvent/scripts/sites/action.greene2020.com/stop-the-steal-rd/default.yml
--rw-r--r--   0        0        0       63 2020-12-31 22:26:05.624955 solvent-23.1.12/solvent/scripts/sites/action.iowagunowners.org/action/re-open-iowa-for-business/default.yml
--rw-r--r--   0        0        0       63 2020-12-31 22:26:05.620194 solvent-23.1.12/solvent/scripts/sites/action.iowagunowners.org/sign-up/default.yml
--rw-r--r--   0        0        0      275 2022-08-21 01:44:58.371700 solvent-23.1.12/solvent/scripts/sites/apps.apple.com/us/app/truth-social/id1586018825/default.yml
--rw-r--r--   0        0        0     2395 2022-08-14 19:37:15.781045 solvent-23.1.12/solvent/scripts/sites/chiefjamescraig.com/@/default.yml
--rw-r--r--   0        0        0     1182 2022-12-04 22:27:38.843544 solvent-23.1.12/solvent/scripts/sites/ci.criticalimpact.com/wc/wc.cfm/default.yml
--rw-r--r--   0        0        0     2186 2020-12-31 22:26:05.809616 solvent-23.1.12/solvent/scripts/sites/defendyourballot.formstack.com/forms/voter_fraud/default.yml
--rw-r--r--   0        0        0      797 2022-12-04 22:04:16.298341 solvent-23.1.12/solvent/scripts/sites/donjr.com/@/default.yml
--rw-r--r--   0        0        0     4841 2021-08-17 19:51:32.987519 solvent-23.1.12/solvent/scripts/sites/donjr.com/challenge/contact_form.yml
--rw-r--r--   0        0        0     1252 2022-08-27 18:47:35.896122 solvent-23.1.12/solvent/scripts/sites/donjr.com/checkouts/c/{c}/information/default.yml
--rw-r--r--   0        0        0      632 2022-08-27 19:19:46.716722 solvent-23.1.12/solvent/scripts/sites/donjr.com/checkouts/c/{c}/payment/default.yml
--rw-r--r--   0        0        0      423 2022-08-27 18:47:40.769360 solvent-23.1.12/solvent/scripts/sites/donjr.com/checkouts/c/{c}/shipping/default.yml
--rw-r--r--   0        0        0     3294 2022-12-04 22:04:26.849319 solvent-23.1.12/solvent/scripts/sites/donjr.com/collections/all/default.yml
--rw-r--r--   0        0        0     8511 2022-12-04 22:04:37.079393 solvent-23.1.12/solvent/scripts/sites/donjr.com/collections/all/products/{slug}/default.yml
--rw-r--r--   0        0        0     2273 2022-08-21 01:44:58.372139 solvent-23.1.12/solvent/scripts/sites/donjr.com/{product}/checkouts/{cart}/default.yml
--rw-r--r--   0        0        0     1079 2022-01-23 17:04:05.513017 solvent-23.1.12/solvent/scripts/sites/fa.ml.com/connecticut/stamford/theiannazzogroup/default.yml
--rw-r--r--   0        0        0     1030 2022-12-17 05:36:09.268092 solvent-23.1.12/solvent/scripts/sites/frankspeech.com/@/default.yml
--rw-r--r--   0        0        0      275 2021-07-09 21:29:35.447127 solvent-23.1.12/solvent/scripts/sites/frankspeech.com/redirect.html/default.yml
--rw-r--r--   0        0        0     3227 2022-12-17 05:36:28.381013 solvent-23.1.12/solvent/scripts/sites/frankspeech.com/user/register/default.yml
--rw-r--r--   0        0        0     2902 2022-01-29 19:12:36.459903 solvent-23.1.12/solvent/scripts/sites/fs10.formsite.com/res/showFormEmbed/default.yml
--rw-r--r--   0        0        0      275 2021-04-17 11:57:33.419480 solvent-23.1.12/solvent/scripts/sites/fs10.formsite.com/res/showSuccessPage/default.yml
--rw-r--r--   0        0        0      275 2021-04-17 11:52:48.464942 solvent-23.1.12/solvent/scripts/sites/fs10.formsite.com/res/submit/default.yml
--rw-r--r--   0        0        0     2782 2022-01-29 18:54:35.222265 solvent-23.1.12/solvent/scripts/sites/fs21.formsite.com/res/showFormEmbed/default.yml
--rw-r--r--   0        0        0      275 2021-04-17 02:50:33.630540 solvent-23.1.12/solvent/scripts/sites/fs21.formsite.com/res/showSuccessPage/default.yml
--rw-r--r--   0        0        0      275 2021-04-17 02:50:33.630786 solvent-23.1.12/solvent/scripts/sites/fs21.formsite.com/res/submit/default.yml
--rw-r--r--   0        0        0     3803 2021-07-09 21:33:29.869501 solvent-23.1.12/solvent/scripts/sites/gettr.com/@/default.yml
--rw-r--r--   0        0        0     1324 2021-07-09 21:42:36.108093 solvent-23.1.12/solvent/scripts/sites/gettr.com/helpcenter/registration/default.yml
--rw-r--r--   0        0        0      275 2021-07-09 21:31:50.704631 solvent-23.1.12/solvent/scripts/sites/gettr.com/signup/default.yml
--rw-r--r--   0        0        0     3714 2022-12-04 22:07:14.029777 solvent-23.1.12/solvent/scripts/sites/helmsoptical.com/@/default.yml
--rw-r--r--   0        0        0     1626 2022-01-29 18:53:11.169783 solvent-23.1.12/solvent/scripts/sites/helmsoptical.com/contact-us/default.yml
--rw-r--r--   0        0        0      275 2022-08-21 01:44:58.372523 solvent-23.1.12/solvent/scripts/sites/help.truthsocial.com/@/default.yml
--rw-r--r--   0        0        0     1167 2022-12-04 22:07:32.390637 solvent-23.1.12/solvent/scripts/sites/heyhandy.xyz/@/default.yml
--rw-r--r--   0        0        0      275 2021-06-05 15:50:59.418661 solvent-23.1.12/solvent/scripts/sites/home.frankspeech.com/@/default.yml
--rw-r--r--   0        0        0     1072 2022-12-04 22:01:26.737127 solvent-23.1.12/solvent/scripts/sites/integrations.salesflare.com/s/tortii/default.yml
--rw-r--r--   0        0        0      290 2021-05-07 01:02:13.550669 solvent-23.1.12/solvent/scripts/sites/iqconnect.lmhostediq.com/iqextranet/EsurveyForm.aspx/default.yml
--rw-r--r--   0        0        0      408 2022-08-28 23:38:09.124620 solvent-23.1.12/solvent/scripts/sites/martinhyde.us/@/default.yml
--rw-r--r--   0        0        0      972 2022-10-27 15:45:31.864298 solvent-23.1.12/solvent/scripts/sites/martinhyde.us/contact/default.yml
--rw-r--r--   0        0        0     1262 2021-03-27 14:07:38.535623 solvent-23.1.12/solvent/scripts/sites/nolabels.salsalabs.org/071020trumphandlingcovid--19/index.html/default.yml
--rw-r--r--   0        0        0      543 2021-08-17 19:54:36.878375 solvent-23.1.12/solvent/scripts/sites/nunes.house.gov/@/default.yml
--rw-r--r--   0        0        0      275 2021-03-27 14:14:48.853708 solvent-23.1.12/solvent/scripts/sites/nunes.house.gov/contact/subscribe.htm/default.yml
--rw-r--r--   0        0        0       63 2020-12-31 22:26:05.914868 solvent-23.1.12/solvent/scripts/sites/oneclickpolitics.global.ssl.fastly.net/messages/edit/default.yml
--rw-r--r--   0        0        0     1689 2022-12-04 22:09:18.404011 solvent-23.1.12/solvent/scripts/sites/patriotpage.org/register/default.yml
--rw-r--r--   0        0        0     1293 2022-12-04 22:08:53.553018 solvent-23.1.12/solvent/scripts/sites/patriotpage.org/wp-login.php/default.yml
--rw-r--r--   0        0        0     1234 2022-08-24 01:08:22.595627 solvent-23.1.12/solvent/scripts/sites/prod-static.frankspeech.com/landing-page.html/default.yml
--rw-r--r--   0        0        0     2375 2022-03-03 22:03:45.513237 solvent-23.1.12/solvent/scripts/sites/professorwatchlist.org/@/default.yml
--rw-r--r--   0        0        0     1457 2021-08-22 15:56:20.494006 solvent-23.1.12/solvent/scripts/sites/prolifewhistleblower.com/anonymous-form/default.yml
--rw-r--r--   0        0        0       63 2020-12-31 22:26:05.903317 solvent-23.1.12/solvent/scripts/sites/rebellegends.org/@/default.yml
--rw-r--r--   0        0        0       63 2020-12-31 22:26:05.824184 solvent-23.1.12/solvent/scripts/sites/reopennc.com/@/default.yml
--rw-r--r--   0        0        0      275 2021-04-10 20:30:23.841208 solvent-23.1.12/solvent/scripts/sites/savannahtaphouse.com/@/default.yml
--rw-r--r--   0        0        0     3387 2021-05-28 14:31:32.869359 solvent-23.1.12/solvent/scripts/sites/savannahtaphouse.com/contact/default.yml
--rw-r--r--   0        0        0       63 2020-12-31 22:26:05.814524 solvent-23.1.12/solvent/scripts/sites/secure.anedot.com/greene-for-congress-inc/stop-the-steal-rd/default.yml
--rw-r--r--   0        0        0       63 2020-12-31 22:26:05.819299 solvent-23.1.12/solvent/scripts/sites/secure.donaldjtrump.com/official-2020-strategy-survey/default.yml
--rw-r--r--   0        0        0      275 2022-02-12 02:02:58.652665 solvent-23.1.12/solvent/scripts/sites/secure.winred.com/james-craig-for-governor/action-lftf-homepage/default.yml
--rw-r--r--   0        0        0      962 2022-08-14 19:37:29.751515 solvent-23.1.12/solvent/scripts/sites/secure.winred.com/james-craig-for-governor/action-lftf-homepage/thank-you/preview/default.yml
--rw-r--r--   0        0        0      275 2021-05-25 23:50:22.809130 solvent-23.1.12/solvent/scripts/sites/secure.winred.com/save-america-joint-fundraising-committee/membership/default.yml
--rw-r--r--   0        0        0     2790 2021-02-04 14:32:12.158437 solvent-23.1.12/solvent/scripts/sites/secure.winred.com/stop-stacey-inc/donate/default.yml
--rw-r--r--   0        0        0      275 2022-12-04 21:42:03.595420 solvent-23.1.12/solvent/scripts/sites/secure.winred.com/stop-stacey-inc/donate/thank-you/preview/default.yml
--rw-r--r--   0        0        0      191 2020-12-31 22:26:05.673675 solvent-23.1.12/solvent/scripts/sites/shop.donaldjtrump.com/@/default.yml
--rw-r--r--   0        0        0       63 2020-12-31 22:26:05.629970 solvent-23.1.12/solvent/scripts/sites/steube.house.gov/@/default.yml
--rw-r--r--   0        0        0      475 2021-03-27 14:20:06.644666 solvent-23.1.12/solvent/scripts/sites/steube.house.gov/contact/newsletter/default.yml
--rw-r--r--   0        0        0       63 2020-12-31 22:26:05.664484 solvent-23.1.12/solvent/scripts/sites/steube.house.gov/contact/newsletter/newsletter-subscribe-thank-you/default.yml
--rw-r--r--   0        0        0      718 2022-12-04 22:27:52.612972 solvent-23.1.12/solvent/scripts/sites/stopstacey.org/@/default.yml
--rw-r--r--   0        0        0      275 2021-12-31 18:12:46.802782 solvent-23.1.12/solvent/scripts/sites/texasrighttolife.com/@/default.yml
--rw-r--r--   0        0        0       63 2020-12-31 22:26:05.678881 solvent-23.1.12/solvent/scripts/sites/trumpvictory.com/free-yard-sign/default.yml
--rw-r--r--   0        0        0     5063 2022-12-17 05:31:57.824535 solvent-23.1.12/solvent/scripts/sites/truthsocial.com/@/default.yml
--rw-r--r--   0        0        0      275 2021-10-27 20:57:52.949106 solvent-23.1.12/solvent/scripts/sites/truthsocial.com/thanks/default.yml
--rw-r--r--   0        0        0      656 2022-12-04 22:32:55.281253 solvent-23.1.12/solvent/scripts/sites/truthsocial.com/verify/default.yml
--rw-r--r--   0        0        0       63 2020-12-31 22:26:05.908739 solvent-23.1.12/solvent/scripts/sites/unlockmichigan.com/thank-you/default.yml
--rw-r--r--   0        0        0       63 2020-12-31 22:26:05.840004 solvent-23.1.12/solvent/scripts/sites/unlockmichigan.ivolunteers.com/Account/Register/default.yml
--rw-r--r--   0        0        0       63 2020-12-31 22:26:05.833931 solvent-23.1.12/solvent/scripts/sites/unlockmichigan.ivolunteers.com/Account/ThankYou/default.yml
--rw-r--r--   0        0        0       63 2020-12-31 22:26:05.846534 solvent-23.1.12/solvent/scripts/sites/unlockmichigan.ivolunteers.com/Error/NotFound/default.yml
--rw-r--r--   0        0        0       63 2020-12-31 22:26:05.829007 solvent-23.1.12/solvent/scripts/sites/unlockmichigan.ivolunteers.com/Register/extrapetitions/default.yml
--rw-r--r--   0        0        0     2806 2021-07-25 03:10:22.639175 solvent-23.1.12/solvent/scripts/sites/www.beckysflowersmidland.com/contacts.html/default.yml
--rw-r--r--   0        0        0      167 2021-01-08 03:30:44.558444 solvent-23.1.12/solvent/scripts/sites/www.beckysflowersmidland.com/index.html/default.yml
--rw-r--r--   0        0        0     1090 2022-12-04 22:35:35.892746 solvent-23.1.12/solvent/scripts/sites/www.cityoftarrant.com/contact/default.yml
--rw-r--r--   0        0        0      275 2021-07-25 05:23:37.332182 solvent-23.1.12/solvent/scripts/sites/www.cityoftarrant.com/node/7/done/default.yml
--rw-r--r--   0        0        0      275 2022-08-21 01:44:58.373652 solvent-23.1.12/solvent/scripts/sites/www.clickfunnels.com/@/default.yml
--rw-r--r--   0        0        0      894 2022-08-28 23:38:56.403137 solvent-23.1.12/solvent/scripts/sites/www.daterightstuff.com/home/default.yml
--rw-r--r--   0        0        0      275 2022-10-11 12:07:39.146956 solvent-23.1.12/solvent/scripts/sites/www.daterightstuff.com/homepagevideo/default.yml
--rw-r--r--   0        0        0      275 2022-12-04 21:54:28.004241 solvent-23.1.12/solvent/scripts/sites/www.daterightstuff.com/optin-565025161664468347967/default.yml
--rw-r--r--   0        0        0      275 2022-08-28 23:09:31.563412 solvent-23.1.12/solvent/scripts/sites/www.daterightstuff.com/thank-you1649518979405/default.yml
--rw-r--r--   0        0        0       63 2020-12-31 22:26:05.522799 solvent-23.1.12/solvent/scripts/sites/www.donaldjtrump.com/@/default.yml
--rw-r--r--   0        0        0      275 2022-01-29 18:55:11.628804 solvent-23.1.12/solvent/scripts/sites/www.donaldjtrump.com/alerts/default.yml
--rw-r--r--   0        0        0     1088 2021-06-02 00:48:56.551974 solvent-23.1.12/solvent/scripts/sites/www.donaldjtrump.com/desk/default.yml
--rw-r--r--   0        0        0     1582 2020-12-31 22:26:05.615262 solvent-23.1.12/solvent/scripts/sites/www.donaldjtrump.com/landing/the-official-2020-strategy-survey/default.yml
--rw-r--r--   0        0        0       63 2020-12-31 22:26:05.749373 solvent-23.1.12/solvent/scripts/sites/www.facebook.com/login.php/default.yml
--rw-r--r--   0        0        0     3199 2022-08-24 01:15:42.517708 solvent-23.1.12/solvent/scripts/sites/www.joinrightstuff.com/home/default.yml
--rw-r--r--   0        0        0      397 2022-08-18 19:47:09.170812 solvent-23.1.12/solvent/scripts/sites/www.joinrightstuff.com/thank-you{id}/default.yml
--rw-r--r--   0        0        0     7545 2021-06-02 16:17:14.274985 solvent-23.1.12/solvent/scripts/sites/www.mackinawcity.net/contact.php/default.yml
--rw-r--r--   0        0        0      275 2021-05-28 14:46:46.746792 solvent-23.1.12/solvent/scripts/sites/www.mackinawcity.net/contact_success.php/default.yml
--rw-r--r--   0        0        0      982 2022-12-04 21:55:02.517887 solvent-23.1.12/solvent/scripts/sites/www.mypillow.com/@/default.yml
--rw-r--r--   0        0        0      275 2022-01-29 19:07:10.336987 solvent-23.1.12/solvent/scripts/sites/www.mypillow.com/subscribe33/default.yml
--rw-r--r--   0        0        0      275 2022-01-29 18:53:11.171366 solvent-23.1.12/solvent/scripts/sites/www.nunes.house.gov/@/default.yml
--rw-r--r--   0        0        0      980 2021-01-09 19:15:01.068405 solvent-23.1.12/solvent/scripts/sites/www.paypal.com/checkoutnow/default.yml
--rw-r--r--   0        0        0     1129 2022-10-27 16:15:28.361091 solvent-23.1.12/solvent/scripts/sites/www.shopfamilyfare.com/@/default.yml
--rw-r--r--   0        0        0      418 2022-10-27 16:15:32.065378 solvent-23.1.12/solvent/scripts/sites/www.shopfamilyfare.com/p/help/default.yml
--rw-r--r--   0        0        0     1986 2023-01-13 00:15:59.999624 solvent-23.1.12/solvent/scripts/sites/www.shopfamilyfare.com/p/help/message/default.yml
--rw-r--r--   0        0        0      275 2021-12-31 18:12:40.719463 solvent-23.1.12/solvent/scripts/sites/www.texasrighttolife.com/join/default.yml
--rw-r--r--   0        0        0     3003 2021-04-17 11:33:57.359077 solvent-23.1.12/solvent/scripts/sites/www.tpaction.com/@/default.yml
--rw-r--r--   0        0        0      275 2021-04-17 11:38:24.126633 solvent-23.1.12/solvent/scripts/sites/www.tpaction.com/pc/default.yml
--rw-r--r--   0        0        0      844 2021-04-17 02:50:33.631254 solvent-23.1.12/solvent/scripts/sites/www.tpusa.com/@/default.yml
--rw-r--r--   0        0        0     1780 2021-04-17 02:50:33.632232 solvent-23.1.12/solvent/scripts/sites/www.tpusa.com/contactus/default.yml
--rw-r--r--   0        0        0      275 2021-10-27 20:54:08.258533 solvent-23.1.12/solvent/scripts/sites/www.truthsocial.com/thanks/default.yml
--rw-r--r--   0        0        0     1367 2022-08-04 18:09:34.318907 solvent-23.1.12/solvent/scripts/sites/www.votejohngibbs.com/@/default.yml
--rw-r--r--   0        0        0     4910 2022-08-04 18:12:42.601913 solvent-23.1.12/solvent/scripts/sites/www.votejohngibbs.com/home/default.yml
--rw-r--r--   0        0        0     2211 2022-12-04 22:11:15.144198 solvent-23.1.12/solvent/scripts/trump.py
--rw-r--r--   0        0        0     7785 1970-01-01 00:00:00.000000 solvent-23.1.12/setup.py
--rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 solvent-23.1.12/PKG-INFO
+-rw-r--r--   0        0        0      883 2023-06-18 21:50:57.765600 solvent-23.6.18/pyproject.toml
+-rw-r--r--   0        0        0       76 2022-06-12 16:52:49.179834 solvent-23.6.18/solvent/__init__.py
+-rw-r--r--   0        0        0       60 2021-03-29 00:25:39.960595 solvent-23.6.18/solvent/__main__.py
+-rw-r--r--   0        0        0     2472 2022-08-18 22:21:39.420685 solvent-23.6.18/solvent/cli.py
+-rw-r--r--   0        0        0      811 2022-09-12 19:06:32.523611 solvent-23.6.18/solvent/gui.py
+-rw-r--r--   0        0        0     1925 2023-06-18 21:00:01.315031 solvent-23.6.18/solvent/scripts/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-18 21:07:28.630779 solvent-23.6.18/solvent/scripts/gop.py
+-rw-r--r--   0        0        0     1869 2023-06-18 21:10:14.266589 solvent-23.6.18/solvent/scripts/lindell.py
+-rw-r--r--   0        0        0     2509 2023-06-18 21:04:29.898390 solvent-23.6.18/solvent/scripts/misc.py
+-rw-r--r--   0        0        0      701 2021-03-29 00:25:39.963842 solvent-23.6.18/solvent/scripts/sites/action.greene2020.com/stop-the-steal-rd/default.yml
+-rw-r--r--   0        0        0       63 2021-03-29 00:25:39.964521 solvent-23.6.18/solvent/scripts/sites/action.iowagunowners.org/action/re-open-iowa-for-business/default.yml
+-rw-r--r--   0        0        0       63 2021-03-29 00:25:39.964926 solvent-23.6.18/solvent/scripts/sites/action.iowagunowners.org/sign-up/default.yml
+-rw-r--r--   0        0        0      275 2022-08-20 23:22:56.110837 solvent-23.6.18/solvent/scripts/sites/apps.apple.com/us/app/truth-social/id1586018825/default.yml
+-rw-r--r--   0        0        0     2395 2022-06-13 20:48:38.768812 solvent-23.6.18/solvent/scripts/sites/chiefjamescraig.com/@/default.yml
+-rw-r--r--   0        0        0     1182 2022-10-15 16:07:36.200235 solvent-23.6.18/solvent/scripts/sites/ci.criticalimpact.com/wc/wc.cfm/default.yml
+-rw-r--r--   0        0        0     2186 2021-03-29 00:25:39.966587 solvent-23.6.18/solvent/scripts/sites/defendyourballot.formstack.com/forms/voter_fraud/default.yml
+-rw-r--r--   0        0        0      797 2023-06-18 21:04:54.824287 solvent-23.6.18/solvent/scripts/sites/donjr.com/@/default.yml
+-rw-r--r--   0        0        0     4841 2022-06-13 20:52:50.773396 solvent-23.6.18/solvent/scripts/sites/donjr.com/challenge/contact_form.yml
+-rw-r--r--   0        0        0     1252 2022-09-29 03:39:05.222102 solvent-23.6.18/solvent/scripts/sites/donjr.com/checkouts/c/{c}/information/default.yml
+-rw-r--r--   0        0        0      632 2022-09-29 04:25:08.566235 solvent-23.6.18/solvent/scripts/sites/donjr.com/checkouts/c/{c}/payment/default.yml
+-rw-r--r--   0        0        0      423 2022-09-29 03:39:10.166686 solvent-23.6.18/solvent/scripts/sites/donjr.com/checkouts/c/{c}/shipping/default.yml
+-rw-r--r--   0        0        0     3294 2023-06-18 21:05:00.799530 solvent-23.6.18/solvent/scripts/sites/donjr.com/collections/all/default.yml
+-rw-r--r--   0        0        0     8511 2023-06-18 21:05:28.534644 solvent-23.6.18/solvent/scripts/sites/donjr.com/collections/all/products/{slug}/default.yml
+-rw-r--r--   0        0        0     2273 2022-08-18 22:21:39.421786 solvent-23.6.18/solvent/scripts/sites/donjr.com/{product}/checkouts/{cart}/default.yml
+-rw-r--r--   0        0        0     1079 2022-01-27 21:02:20.443439 solvent-23.6.18/solvent/scripts/sites/fa.ml.com/connecticut/stamford/theiannazzogroup/default.yml
+-rw-r--r--   0        0        0     1030 2023-06-18 21:19:35.041635 solvent-23.6.18/solvent/scripts/sites/frankspeech.com/@/default.yml
+-rw-r--r--   0        0        0      275 2021-06-05 17:22:44.800385 solvent-23.6.18/solvent/scripts/sites/frankspeech.com/redirect.html/default.yml
+-rw-r--r--   0        0        0     3228 2023-06-18 21:19:39.717339 solvent-23.6.18/solvent/scripts/sites/frankspeech.com/user/register/default.yml
+-rw-r--r--   0        0        0     2902 2022-01-29 19:20:49.402029 solvent-23.6.18/solvent/scripts/sites/fs10.formsite.com/res/showFormEmbed/default.yml
+-rw-r--r--   0        0        0      275 2021-04-17 16:23:20.229033 solvent-23.6.18/solvent/scripts/sites/fs10.formsite.com/res/showSuccessPage/default.yml
+-rw-r--r--   0        0        0      275 2021-04-17 16:23:20.229434 solvent-23.6.18/solvent/scripts/sites/fs10.formsite.com/res/submit/default.yml
+-rw-r--r--   0        0        0     2782 2022-01-29 19:20:49.402444 solvent-23.6.18/solvent/scripts/sites/fs21.formsite.com/res/showFormEmbed/default.yml
+-rw-r--r--   0        0        0      275 2021-04-16 22:39:06.507278 solvent-23.6.18/solvent/scripts/sites/fs21.formsite.com/res/showSuccessPage/default.yml
+-rw-r--r--   0        0        0      275 2021-04-16 22:22:45.040726 solvent-23.6.18/solvent/scripts/sites/fs21.formsite.com/res/submit/default.yml
+-rw-r--r--   0        0        0     3803 2021-07-22 15:29:29.361086 solvent-23.6.18/solvent/scripts/sites/gettr.com/@/default.yml
+-rw-r--r--   0        0        0     1324 2021-07-22 15:29:29.361648 solvent-23.6.18/solvent/scripts/sites/gettr.com/helpcenter/registration/default.yml
+-rw-r--r--   0        0        0      275 2021-07-22 15:29:29.362196 solvent-23.6.18/solvent/scripts/sites/gettr.com/signup/default.yml
+-rw-r--r--   0        0        0     3714 2022-11-14 02:09:57.614549 solvent-23.6.18/solvent/scripts/sites/helmsoptical.com/@/default.yml
+-rw-r--r--   0        0        0     1626 2022-01-28 00:53:33.055835 solvent-23.6.18/solvent/scripts/sites/helmsoptical.com/contact-us/default.yml
+-rw-r--r--   0        0        0      275 2022-08-20 23:23:18.802053 solvent-23.6.18/solvent/scripts/sites/help.truthsocial.com/@/default.yml
+-rw-r--r--   0        0        0     1167 2023-01-18 17:16:19.630403 solvent-23.6.18/solvent/scripts/sites/heyhandy.xyz/@/default.yml
+-rw-r--r--   0        0        0      275 2021-06-05 16:44:07.637929 solvent-23.6.18/solvent/scripts/sites/home.frankspeech.com/@/default.yml
+-rw-r--r--   0        0        0     1072 2023-01-18 17:16:19.632618 solvent-23.6.18/solvent/scripts/sites/integrations.salesflare.com/s/tortii/default.yml
+-rw-r--r--   0        0        0      290 2021-08-04 05:26:36.129059 solvent-23.6.18/solvent/scripts/sites/iqconnect.lmhostediq.com/iqextranet/EsurveyForm.aspx/default.yml
+-rw-r--r--   0        0        0      408 2022-10-15 16:12:29.723313 solvent-23.6.18/solvent/scripts/sites/martinhyde.us/@/default.yml
+-rw-r--r--   0        0        0      972 2022-10-15 16:12:39.080956 solvent-23.6.18/solvent/scripts/sites/martinhyde.us/contact/default.yml
+-rw-r--r--   0        0        0     1262 2021-03-29 00:25:39.977186 solvent-23.6.18/solvent/scripts/sites/nolabels.salsalabs.org/071020trumphandlingcovid--19/index.html/default.yml
+-rw-r--r--   0        0        0      543 2021-08-08 20:12:45.994230 solvent-23.6.18/solvent/scripts/sites/nunes.house.gov/@/default.yml
+-rw-r--r--   0        0        0      275 2021-03-29 00:25:39.978978 solvent-23.6.18/solvent/scripts/sites/nunes.house.gov/contact/subscribe.htm/default.yml
+-rw-r--r--   0        0        0       63 2021-03-29 00:25:39.979702 solvent-23.6.18/solvent/scripts/sites/oneclickpolitics.global.ssl.fastly.net/messages/edit/default.yml
+-rw-r--r--   0        0        0     1689 2023-06-18 21:17:39.154301 solvent-23.6.18/solvent/scripts/sites/patriotpage.org/register/default.yml
+-rw-r--r--   0        0        0     1293 2023-06-18 21:17:21.179176 solvent-23.6.18/solvent/scripts/sites/patriotpage.org/wp-login.php/default.yml
+-rw-r--r--   0        0        0     1234 2022-08-24 21:58:24.296774 solvent-23.6.18/solvent/scripts/sites/prod-static.frankspeech.com/landing-page.html/default.yml
+-rw-r--r--   0        0        0     2375 2022-04-02 03:52:35.494154 solvent-23.6.18/solvent/scripts/sites/professorwatchlist.org/@/default.yml
+-rw-r--r--   0        0        0     1457 2021-10-31 14:58:05.934654 solvent-23.6.18/solvent/scripts/sites/prolifewhistleblower.com/anonymous-form/default.yml
+-rw-r--r--   0        0        0       63 2021-03-29 00:25:39.980151 solvent-23.6.18/solvent/scripts/sites/rebellegends.org/@/default.yml
+-rw-r--r--   0        0        0       63 2021-03-29 00:25:39.980605 solvent-23.6.18/solvent/scripts/sites/reopennc.com/@/default.yml
+-rw-r--r--   0        0        0      275 2021-04-16 21:42:11.606953 solvent-23.6.18/solvent/scripts/sites/savannahtaphouse.com/@/default.yml
+-rw-r--r--   0        0        0     3387 2021-05-30 14:40:11.081245 solvent-23.6.18/solvent/scripts/sites/savannahtaphouse.com/contact/default.yml
+-rw-r--r--   0        0        0       63 2021-03-29 00:25:39.981166 solvent-23.6.18/solvent/scripts/sites/secure.anedot.com/greene-for-congress-inc/stop-the-steal-rd/default.yml
+-rw-r--r--   0        0        0       63 2021-03-29 00:25:39.981579 solvent-23.6.18/solvent/scripts/sites/secure.donaldjtrump.com/official-2020-strategy-survey/default.yml
+-rw-r--r--   0        0        0      275 2022-04-02 03:52:35.494699 solvent-23.6.18/solvent/scripts/sites/secure.winred.com/james-craig-for-governor/action-lftf-homepage/default.yml
+-rw-r--r--   0        0        0      962 2022-08-16 23:14:13.972152 solvent-23.6.18/solvent/scripts/sites/secure.winred.com/james-craig-for-governor/action-lftf-homepage/thank-you/preview/default.yml
+-rw-r--r--   0        0        0      275 2021-05-26 00:22:14.908362 solvent-23.6.18/solvent/scripts/sites/secure.winred.com/save-america-joint-fundraising-committee/membership/default.yml
+-rw-r--r--   0        0        0     2790 2022-09-29 05:06:58.474167 solvent-23.6.18/solvent/scripts/sites/secure.winred.com/stop-stacey-inc/donate/default.yml
+-rw-r--r--   0        0        0      275 2023-01-18 17:16:19.633339 solvent-23.6.18/solvent/scripts/sites/secure.winred.com/stop-stacey-inc/donate/thank-you/preview/default.yml
+-rw-r--r--   0        0        0      191 2021-03-29 00:25:39.983095 solvent-23.6.18/solvent/scripts/sites/shop.donaldjtrump.com/@/default.yml
+-rw-r--r--   0        0        0       63 2021-03-29 00:25:39.983535 solvent-23.6.18/solvent/scripts/sites/steube.house.gov/@/default.yml
+-rw-r--r--   0        0        0      475 2021-03-29 00:25:39.984242 solvent-23.6.18/solvent/scripts/sites/steube.house.gov/contact/newsletter/default.yml
+-rw-r--r--   0        0        0       63 2021-03-29 00:25:39.984533 solvent-23.6.18/solvent/scripts/sites/steube.house.gov/contact/newsletter/newsletter-subscribe-thank-you/default.yml
+-rw-r--r--   0        0        0      718 2023-06-18 21:06:48.569047 solvent-23.6.18/solvent/scripts/sites/stopstacey.org/@/default.yml
+-rw-r--r--   0        0        0      275 2022-01-29 00:03:29.259461 solvent-23.6.18/solvent/scripts/sites/texasrighttolife.com/@/default.yml
+-rw-r--r--   0        0        0       63 2021-03-29 00:25:39.985747 solvent-23.6.18/solvent/scripts/sites/trumpvictory.com/free-yard-sign/default.yml
+-rw-r--r--   0        0        0     4281 2023-06-18 21:21:40.713551 solvent-23.6.18/solvent/scripts/sites/truthsocial.com/@/default.yml
+-rw-r--r--   0        0        0      275 2021-10-31 14:58:05.936113 solvent-23.6.18/solvent/scripts/sites/truthsocial.com/thanks/default.yml
+-rw-r--r--   0        0        0      656 2023-06-18 21:21:44.995019 solvent-23.6.18/solvent/scripts/sites/truthsocial.com/verify/default.yml
+-rw-r--r--   0        0        0       63 2021-03-29 00:25:39.986127 solvent-23.6.18/solvent/scripts/sites/unlockmichigan.com/thank-you/default.yml
+-rw-r--r--   0        0        0       63 2021-03-29 00:25:39.986766 solvent-23.6.18/solvent/scripts/sites/unlockmichigan.ivolunteers.com/Account/Register/default.yml
+-rw-r--r--   0        0        0       63 2021-03-29 00:25:39.987057 solvent-23.6.18/solvent/scripts/sites/unlockmichigan.ivolunteers.com/Account/ThankYou/default.yml
+-rw-r--r--   0        0        0       63 2021-03-29 00:25:39.987425 solvent-23.6.18/solvent/scripts/sites/unlockmichigan.ivolunteers.com/Error/NotFound/default.yml
+-rw-r--r--   0        0        0       63 2021-03-29 00:25:39.987803 solvent-23.6.18/solvent/scripts/sites/unlockmichigan.ivolunteers.com/Register/extrapetitions/default.yml
+-rw-r--r--   0        0        0     2806 2021-07-24 22:04:01.947642 solvent-23.6.18/solvent/scripts/sites/www.beckysflowersmidland.com/contacts.html/default.yml
+-rw-r--r--   0        0        0      167 2021-03-29 00:25:39.989044 solvent-23.6.18/solvent/scripts/sites/www.beckysflowersmidland.com/index.html/default.yml
+-rw-r--r--   0        0        0     1090 2023-06-18 21:18:18.389467 solvent-23.6.18/solvent/scripts/sites/www.cityoftarrant.com/contact/default.yml
+-rw-r--r--   0        0        0      275 2021-07-22 15:29:29.363180 solvent-23.6.18/solvent/scripts/sites/www.cityoftarrant.com/node/7/done/default.yml
+-rw-r--r--   0        0        0      275 2022-08-18 21:24:05.067451 solvent-23.6.18/solvent/scripts/sites/www.clickfunnels.com/@/default.yml
+-rw-r--r--   0        0        0      894 2022-09-29 15:04:05.597280 solvent-23.6.18/solvent/scripts/sites/www.daterightstuff.com/home/default.yml
+-rw-r--r--   0        0        0      275 2022-10-15 15:09:25.278552 solvent-23.6.18/solvent/scripts/sites/www.daterightstuff.com/homepagevideo/default.yml
+-rw-r--r--   0        0        0      275 2023-01-18 17:16:19.634150 solvent-23.6.18/solvent/scripts/sites/www.daterightstuff.com/optin-565025161664468347967/default.yml
+-rw-r--r--   0        0        0      275 2022-09-12 19:06:32.527365 solvent-23.6.18/solvent/scripts/sites/www.daterightstuff.com/thank-you1649518979405/default.yml
+-rw-r--r--   0        0        0       63 2021-03-29 00:25:39.989770 solvent-23.6.18/solvent/scripts/sites/www.donaldjtrump.com/@/default.yml
+-rw-r--r--   0        0        0      275 2022-01-29 17:42:53.657163 solvent-23.6.18/solvent/scripts/sites/www.donaldjtrump.com/alerts/default.yml
+-rw-r--r--   0        0        0     1088 2021-06-01 22:51:01.390466 solvent-23.6.18/solvent/scripts/sites/www.donaldjtrump.com/desk/default.yml
+-rw-r--r--   0        0        0     1582 2021-03-29 00:25:39.990273 solvent-23.6.18/solvent/scripts/sites/www.donaldjtrump.com/landing/the-official-2020-strategy-survey/default.yml
+-rw-r--r--   0        0        0       63 2021-03-29 00:25:39.990784 solvent-23.6.18/solvent/scripts/sites/www.facebook.com/login.php/default.yml
+-rw-r--r--   0        0        0     3199 2022-08-21 18:30:38.532789 solvent-23.6.18/solvent/scripts/sites/www.joinrightstuff.com/home/default.yml
+-rw-r--r--   0        0        0      397 2022-08-18 19:58:01.436596 solvent-23.6.18/solvent/scripts/sites/www.joinrightstuff.com/thank-you{id}/default.yml
+-rw-r--r--   0        0        0     7545 2021-06-01 22:39:05.862851 solvent-23.6.18/solvent/scripts/sites/www.mackinawcity.net/contact.php/default.yml
+-rw-r--r--   0        0        0      275 2021-05-28 14:58:05.237376 solvent-23.6.18/solvent/scripts/sites/www.mackinawcity.net/contact_success.php/default.yml
+-rw-r--r--   0        0        0      982 2023-06-18 21:59:20.199755 solvent-23.6.18/solvent/scripts/sites/www.mypillow.com/@/default.yml
+-rw-r--r--   0        0        0      275 2022-01-29 19:20:40.877874 solvent-23.6.18/solvent/scripts/sites/www.mypillow.com/subscribe33/default.yml
+-rw-r--r--   0        0        0      275 2022-01-29 17:36:08.013928 solvent-23.6.18/solvent/scripts/sites/www.nunes.house.gov/@/default.yml
+-rw-r--r--   0        0        0      980 2021-03-29 00:25:39.991887 solvent-23.6.18/solvent/scripts/sites/www.paypal.com/checkoutnow/default.yml
+-rw-r--r--   0        0        0     1129 2022-10-27 16:25:21.179424 solvent-23.6.18/solvent/scripts/sites/www.shopfamilyfare.com/@/default.yml
+-rw-r--r--   0        0        0      418 2022-10-27 16:25:21.179997 solvent-23.6.18/solvent/scripts/sites/www.shopfamilyfare.com/p/help/default.yml
+-rw-r--r--   0        0        0     1986 2022-10-29 16:14:00.271740 solvent-23.6.18/solvent/scripts/sites/www.shopfamilyfare.com/p/help/message/default.yml
+-rw-r--r--   0        0        0      275 2022-01-20 05:36:54.807104 solvent-23.6.18/solvent/scripts/sites/www.texasrighttolife.com/join/default.yml
+-rw-r--r--   0        0        0     3003 2021-04-17 16:23:20.231617 solvent-23.6.18/solvent/scripts/sites/www.tpaction.com/@/default.yml
+-rw-r--r--   0        0        0      275 2021-04-17 16:23:20.232044 solvent-23.6.18/solvent/scripts/sites/www.tpaction.com/pc/default.yml
+-rw-r--r--   0        0        0      844 2021-04-16 22:08:13.009875 solvent-23.6.18/solvent/scripts/sites/www.tpusa.com/@/default.yml
+-rw-r--r--   0        0        0     1780 2021-04-16 22:13:28.710404 solvent-23.6.18/solvent/scripts/sites/www.tpusa.com/contactus/default.yml
+-rw-r--r--   0        0        0      275 2021-10-31 14:58:05.936929 solvent-23.6.18/solvent/scripts/sites/www.truthsocial.com/thanks/default.yml
+-rw-r--r--   0        0        0     1367 2022-08-16 23:14:13.973881 solvent-23.6.18/solvent/scripts/sites/www.votejohngibbs.com/@/default.yml
+-rw-r--r--   0        0        0     4910 2022-08-16 23:14:13.974196 solvent-23.6.18/solvent/scripts/sites/www.votejohngibbs.com/home/default.yml
+-rw-r--r--   0        0        0      625 2023-06-18 21:16:14.369223 solvent-23.6.18/solvent/scripts/trump.py
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 solvent-23.6.18/PKG-INFO
```

### Comparing `solvent-23.1.12/pyproject.toml` & `solvent-23.6.18/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 
 name = "solvent"
-version = "23.01.12" # <year>.<month>.<day>[.post<build>]
+version = "23.06.18" # <year>.<month>.<day>[.post<build>]
 description = "Kills off fake grass."
 authors = ["Solvent <solvent@example.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 
-python = "^3.8 <3.11"
+python = "^3.9 <3.12"
 
-pomace = "~0.12"
+pomace = "~0.12.2"
 # pomace = { path = "../pomace", develop = true }
 
 caffeine = { version = "~0.5", platform = "darwin" }
-flet = "^0.1.54"
-typer = "~0.4"
+flet = "^0.7.4"
+typer = "~0.9"
 
 [tool.poetry.dev-dependencies]
 
-autoflake = "^1.3.1"
-black = "^22.1"
-isort = "^5.10"
-mypy = "~0.900"
+autoflake = "^2.1"
+black = "^23.3"
+isort = "^5.12"
+mypy = "^1.3"
 
-pyinstaller = "^5.3"
+pyinstaller = "^5.12"
 
 [tool.black]
 
 quiet = true
 
 [tool.isort]
```

### Comparing `solvent-23.1.12/solvent/cli.py` & `solvent-23.6.18/solvent/cli.py`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/gui.py` & `solvent-23.6.18/solvent/gui.py`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/__init__.py` & `solvent-23.6.18/solvent/scripts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from abc import ABC, abstractmethod
 from time import time
 
 import pomace
 
 
 class Script(ABC):
-
     URL = ""
     SKIP = False
 
     attempted = completed = failed = 0
 
     @property
     def name(self) -> str:
```

### Comparing `solvent-23.1.12/solvent/scripts/lindell.py` & `solvent-23.6.18/solvent/scripts/lindell.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import log
 import pomace
 
 from . import Script
 
 
 class MyPillow(Script):
-
     URL = "https://www.mypillow.com/"
 
     def run(self, page: pomace.Page) -> pomace.Page:
         person = pomace.fake.person
 
         pomace.shared.client.clear_cookies()
         page = pomace.visit(self.URL)
@@ -36,15 +35,14 @@
         success = "Thanks!" in page
         if success:
             page.click_continue_shopping(wait=0)
         return success
 
 
 class FrankSpeech(Script):
-
     URL = "https://frankspeech.com/"
     SKIP = True
 
     def run(self, page: pomace.Page) -> pomace.Page:
         person = pomace.fake.person
 
         if "Access denied" in page:
@@ -60,8 +58,8 @@
         # TODO: Get this working
         # page.fill_password(person.password)
         # page.fill_confirm_password(person.password)
 
         return page.click_create_new_account()
 
     def check(self, page: pomace.Page) -> bool:
-        return "prod-static" not in page.url
+        return "prod-static" not in page.url and "Access denied" not in page
```

### Comparing `solvent-23.1.12/solvent/scripts/sites/action.greene2020.com/stop-the-steal-rd/default.yml` & `solvent-23.6.18/solvent/scripts/sites/action.greene2020.com/stop-the-steal-rd/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/chiefjamescraig.com/@/default.yml` & `solvent-23.6.18/solvent/scripts/sites/chiefjamescraig.com/@/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/ci.criticalimpact.com/wc/wc.cfm/default.yml` & `solvent-23.6.18/solvent/scripts/sites/ci.criticalimpact.com/wc/wc.cfm/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/defendyourballot.formstack.com/forms/voter_fraud/default.yml` & `solvent-23.6.18/solvent/scripts/sites/defendyourballot.formstack.com/forms/voter_fraud/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/donjr.com/@/default.yml` & `solvent-23.6.18/solvent/scripts/sites/donjr.com/@/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/donjr.com/challenge/contact_form.yml` & `solvent-23.6.18/solvent/scripts/sites/donjr.com/challenge/contact_form.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/donjr.com/checkouts/c/{c}/information/default.yml` & `solvent-23.6.18/solvent/scripts/sites/donjr.com/checkouts/c/{c}/information/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/donjr.com/checkouts/c/{c}/payment/default.yml` & `solvent-23.6.18/solvent/scripts/sites/donjr.com/checkouts/c/{c}/payment/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/donjr.com/collections/all/default.yml` & `solvent-23.6.18/solvent/scripts/sites/donjr.com/collections/all/default.yml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         uses: 99
   - verb: click
     name: buy_it_now
     locators:
       - mode: text
         value: Buy it now
         index: 0
-        uses: 59
+        uses: 58
   - verb: click
     name: change
     locators:
       - mode: ''
         value: ''
         index: 0
         uses: 0
```

### Comparing `solvent-23.1.12/solvent/scripts/sites/donjr.com/collections/all/products/{slug}/default.yml` & `solvent-23.6.18/solvent/scripts/sites/donjr.com/collections/all/products/{slug}/default.yml`

 * *Files 4% similar despite different names*

```diff
@@ -78,78 +78,78 @@
       - mode: ''
         value: ''
         index: 0
         uses: 0
       - mode: name
         value: email
         index: 0
-        uses: -40
+        uses: -41
       - mode: name
         value: email
         index: 0
-        uses: -40
+        uses: -41
       - mode: id
         value: email
         index: 0
-        uses: -40
+        uses: -41
       - mode: id
         value: email
         index: 0
-        uses: -40
+        uses: -41
       - mode: css
         value: '[aria-label="Email"]'
         index: 0
-        uses: -40
+        uses: -41
       - mode: id
         value: Email
         index: 0
-        uses: -40
+        uses: -41
       - mode: id
         value: checkout_email_or_phone
         index: 0
-        uses: -40
+        uses: -41
       - mode: id
         value: checkout_email_or_phone
         index: 0
-        uses: -40
+        uses: -41
   - verb: fill
     name: first_name
     locators:
       - mode: ''
         value: ''
         index: 0
         uses: 0
       - mode: name
         value: first_name
         index: 0
-        uses: -40
+        uses: -41
       - mode: name
         value: first-name
         index: 0
-        uses: -40
+        uses: -41
       - mode: id
         value: first_name
         index: 0
-        uses: -40
+        uses: -41
       - mode: id
         value: first-name
         index: 0
-        uses: -40
+        uses: -41
       - mode: css
         value: '[aria-label="First Name"]'
         index: 0
-        uses: -40
+        uses: -41
       - mode: id
         value: FirstName
         index: 0
-        uses: -40
+        uses: -41
       - mode: id
         value: checkout_shipping_address_first_name
         index: 0
-        uses: -40
+        uses: -41
   - verb: fill
     name: last_name
     locators:
       - mode: ''
         value: ''
         index: 0
         uses: 0
@@ -256,27 +256,27 @@
       - mode: ''
         value: ''
         index: 0
         uses: 0
       - mode: text
         value: Change
         index: 0
-        uses: -41
+        uses: -42
       - mode: text
         value: Change
         index: 0
-        uses: -41
+        uses: -42
       - mode: value
         value: Change
         index: 0
-        uses: -41
+        uses: -42
       - mode: value
         value: Change
         index: 0
-        uses: -41
+        uses: -42
   - verb: click
     name: buy_it_now
     locators:
       - mode: text
         value: Buy it now
         index: 0
         uses: 98
```

### Comparing `solvent-23.1.12/solvent/scripts/sites/donjr.com/{product}/checkouts/{cart}/default.yml` & `solvent-23.6.18/solvent/scripts/sites/donjr.com/{product}/checkouts/{cart}/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/fa.ml.com/connecticut/stamford/theiannazzogroup/default.yml` & `solvent-23.6.18/solvent/scripts/sites/fa.ml.com/connecticut/stamford/theiannazzogroup/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/frankspeech.com/@/default.yml` & `solvent-23.6.18/solvent/scripts/sites/frankspeech.com/@/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/frankspeech.com/user/register/default.yml` & `solvent-23.6.18/solvent/scripts/sites/frankspeech.com/user/register/default.yml`

 * *Files 4% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         uses: 2
   - verb: click
     name: create_new_account
     locators:
       - mode: text
         value: Create new account
         index: 0
-        uses: 2
+        uses: 1
   - verb: click
     name: accept
     locators:
       - mode: id
         value: edit-field-phone-confirm-value
         index: 0
         uses: 2
@@ -123,50 +123,50 @@
         uses: 0
   - verb: click
     name: confirm
     locators:
       - mode: id
         value: edit-field-phone-confirm-value
         index: 0
-        uses: 1
+        uses: 0
   - verb: fill
     name: phone
     locators:
       - mode: id
         value: edit-field-phone-number-0-value
         index: 0
-        uses: 1
+        uses: -1
   - verb: fill
     name: email
     locators:
       - mode: ''
         value: ''
         index: 0
         uses: 0
       - mode: name
         value: email
         index: 0
-        uses: -4
+        uses: -6
       - mode: name
         value: email
         index: 0
-        uses: -4
+        uses: -6
       - mode: id
         value: email
         index: 0
-        uses: -4
+        uses: -6
       - mode: id
         value: email
         index: 0
-        uses: -4
+        uses: -6
       - mode: aria-label
         value: Email
         index: 0
-        uses: -4
+        uses: -6
       - mode: css
         value: '[placeholder="Email"]'
         index: 0
-        uses: -4
+        uses: -6
       - mode: id
         value: Email
         index: 0
-        uses: -4
+        uses: -6
```

### Comparing `solvent-23.1.12/solvent/scripts/sites/fs10.formsite.com/res/showFormEmbed/default.yml` & `solvent-23.6.18/solvent/scripts/sites/fs10.formsite.com/res/showFormEmbed/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/fs21.formsite.com/res/showFormEmbed/default.yml` & `solvent-23.6.18/solvent/scripts/sites/fs21.formsite.com/res/showFormEmbed/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/gettr.com/@/default.yml` & `solvent-23.6.18/solvent/scripts/sites/gettr.com/@/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/gettr.com/helpcenter/registration/default.yml` & `solvent-23.6.18/solvent/scripts/sites/gettr.com/helpcenter/registration/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/helmsoptical.com/@/default.yml` & `solvent-23.6.18/solvent/scripts/sites/helmsoptical.com/@/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/helmsoptical.com/contact-us/default.yml` & `solvent-23.6.18/solvent/scripts/sites/helmsoptical.com/contact-us/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/heyhandy.xyz/@/default.yml` & `solvent-23.6.18/solvent/scripts/sites/heyhandy.xyz/@/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/integrations.salesflare.com/s/tortii/default.yml` & `solvent-23.6.18/solvent/scripts/sites/integrations.salesflare.com/s/tortii/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/martinhyde.us/contact/default.yml` & `solvent-23.6.18/solvent/scripts/sites/martinhyde.us/contact/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/nolabels.salsalabs.org/071020trumphandlingcovid--19/index.html/default.yml` & `solvent-23.6.18/solvent/scripts/sites/nolabels.salsalabs.org/071020trumphandlingcovid--19/index.html/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/nunes.house.gov/@/default.yml` & `solvent-23.6.18/solvent/scripts/sites/nunes.house.gov/@/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/patriotpage.org/register/default.yml` & `solvent-23.6.18/solvent/scripts/sites/patriotpage.org/register/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/patriotpage.org/wp-login.php/default.yml` & `solvent-23.6.18/solvent/scripts/sites/patriotpage.org/wp-login.php/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/prod-static.frankspeech.com/landing-page.html/default.yml` & `solvent-23.6.18/solvent/scripts/sites/prod-static.frankspeech.com/landing-page.html/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/professorwatchlist.org/@/default.yml` & `solvent-23.6.18/solvent/scripts/sites/professorwatchlist.org/@/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/prolifewhistleblower.com/anonymous-form/default.yml` & `solvent-23.6.18/solvent/scripts/sites/prolifewhistleblower.com/anonymous-form/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/savannahtaphouse.com/contact/default.yml` & `solvent-23.6.18/solvent/scripts/sites/savannahtaphouse.com/contact/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/secure.winred.com/james-craig-for-governor/action-lftf-homepage/thank-you/preview/default.yml` & `solvent-23.6.18/solvent/scripts/sites/secure.winred.com/james-craig-for-governor/action-lftf-homepage/thank-you/preview/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/secure.winred.com/stop-stacey-inc/donate/default.yml` & `solvent-23.6.18/solvent/scripts/sites/secure.winred.com/stop-stacey-inc/donate/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/stopstacey.org/@/default.yml` & `solvent-23.6.18/solvent/scripts/sites/stopstacey.org/@/default.yml`

 * *Files 3% similar despite different names*

```diff
@@ -19,26 +19,26 @@
         uses: 0
   - verb: fill
     name: email
     locators:
       - mode: name
         value: CI_email
         index: 0
-        uses: 99
+        uses: 96
   - verb: fill
     name: zip
     locators:
       - mode: name
         value: CI_custom2
         index: 0
-        uses: 98
+        uses: 95
   - verb: click
     name: submit
     locators:
       - mode: value
         value: Submit
         index: 1
-        uses: 25
+        uses: 22
       - mode: id
         value: CI_submit
         index: 0
-        uses: 50
+        uses: 47
```

### Comparing `solvent-23.1.12/solvent/scripts/sites/truthsocial.com/@/default.yml` & `solvent-23.6.18/solvent/scripts/sites/truthsocial.com/@/default.yml`

 * *Files 15% similar despite different names*

```diff
@@ -218,47 +218,11 @@
       - mode: text (partial)
         value: help center
         index: 0
         uses: 0
   - verb: click
     name: create_an_account
     locators:
-      - mode: ''
-        value: ''
-        index: 0
-        uses: 0
-      - mode: text
-        value: Create An Account
-        index: 0
-        uses: -1
       - mode: text
         value: Create an account
         index: 0
         uses: 2
-      - mode: text
-        value: create an account
-        index: 0
-        uses: 0
-      - mode: value
-        value: Create An Account
-        index: 0
-        uses: 0
-      - mode: value
-        value: Create an account
-        index: 0
-        uses: 0
-      - mode: value
-        value: create an account
-        index: 0
-        uses: 0
-      - mode: text (partial)
-        value: Create An Account
-        index: 0
-        uses: 0
-      - mode: text (partial)
-        value: Create an account
-        index: 0
-        uses: 0
-      - mode: text (partial)
-        value: create an account
-        index: 0
-        uses: 0
```

### Comparing `solvent-23.1.12/solvent/scripts/sites/truthsocial.com/verify/default.yml` & `solvent-23.6.18/solvent/scripts/sites/truthsocial.com/verify/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/www.beckysflowersmidland.com/contacts.html/default.yml` & `solvent-23.6.18/solvent/scripts/sites/www.beckysflowersmidland.com/contacts.html/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/www.cityoftarrant.com/contact/default.yml` & `solvent-23.6.18/solvent/scripts/sites/www.cityoftarrant.com/contact/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/www.daterightstuff.com/home/default.yml` & `solvent-23.6.18/solvent/scripts/sites/www.daterightstuff.com/home/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/www.donaldjtrump.com/desk/default.yml` & `solvent-23.6.18/solvent/scripts/sites/www.donaldjtrump.com/desk/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/www.donaldjtrump.com/landing/the-official-2020-strategy-survey/default.yml` & `solvent-23.6.18/solvent/scripts/sites/www.donaldjtrump.com/landing/the-official-2020-strategy-survey/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/www.joinrightstuff.com/home/default.yml` & `solvent-23.6.18/solvent/scripts/sites/www.joinrightstuff.com/home/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/www.mackinawcity.net/contact.php/default.yml` & `solvent-23.6.18/solvent/scripts/sites/www.mackinawcity.net/contact.php/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/www.mypillow.com/@/default.yml` & `solvent-23.6.18/solvent/scripts/sites/www.mypillow.com/@/default.yml`

 * *Files 2% similar despite different names*

```diff
@@ -13,43 +13,43 @@
         uses: 0
   - verb: fill
     name: phone
     locators:
       - mode: id
         value: ltkpopup-mobile
         index: 0
-        uses: 0
+        uses: 2
   - verb: click
     name: submit
     locators:
       - mode: id
         value: ltkpopup-submit
         index: 0
         uses: 88
   - verb: fill
     name: email_address
     locators:
       - mode: id
         value: ltkpopup-email
         index: 0
-        uses: 0
+        uses: 2
   - verb: click
     name: activate_offer
     locators:
       - mode: value
         value: Activate Offer
         index: 0
-        uses: 0
+        uses: 2
   - verb: click
     name: get_mobile_alerts
     locators:
       - mode: id
         value: ltkpopup-mobile-submit
         index: 0
-        uses: 0
+        uses: 2
   - verb: click
     name: continue_shopping
     locators:
       - mode: text
         value: Continue Shopping
         index: 0
         uses: 2
```

### Comparing `solvent-23.1.12/solvent/scripts/sites/www.paypal.com/checkoutnow/default.yml` & `solvent-23.6.18/solvent/scripts/sites/www.paypal.com/checkoutnow/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/www.shopfamilyfare.com/@/default.yml` & `solvent-23.6.18/solvent/scripts/sites/www.shopfamilyfare.com/@/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/www.shopfamilyfare.com/p/help/message/default.yml` & `solvent-23.6.18/solvent/scripts/sites/www.shopfamilyfare.com/p/help/message/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/www.tpaction.com/@/default.yml` & `solvent-23.6.18/solvent/scripts/sites/www.tpaction.com/@/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/www.tpusa.com/@/default.yml` & `solvent-23.6.18/solvent/scripts/sites/www.tpusa.com/@/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/www.tpusa.com/contactus/default.yml` & `solvent-23.6.18/solvent/scripts/sites/www.tpusa.com/contactus/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/www.votejohngibbs.com/@/default.yml` & `solvent-23.6.18/solvent/scripts/sites/www.votejohngibbs.com/@/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/solvent/scripts/sites/www.votejohngibbs.com/home/default.yml` & `solvent-23.6.18/solvent/scripts/sites/www.votejohngibbs.com/home/default.yml`

 * *Files identical despite different names*

### Comparing `solvent-23.1.12/PKG-INFO` & `solvent-23.6.18/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: solvent
-Version: 23.1.12
+Version: 23.6.18
 Summary: Kills off fake grass.
 License: MIT
 Author: Solvent
 Author-email: solvent@example.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: caffeine (>=0.5,<0.6) ; sys_platform == "darwin"
-Requires-Dist: flet (>=0.1.54,<0.2.0)
-Requires-Dist: pomace (>=0.12,<0.13)
-Requires-Dist: typer (>=0.4,<0.5)
+Requires-Dist: flet (>=0.7.4,<0.8.0)
+Requires-Dist: pomace (>=0.12.2,<0.13.0)
+Requires-Dist: typer (>=0.9,<0.10)
```

