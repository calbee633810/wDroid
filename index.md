# A Tale of Two Cities:How WebView Induces Bugs to Android Applications

In our empirical study, we collected 126 WebView-induced bugs from 51 popular open-source Android apps. We aim to understand their root causes, bug consequences, and manifestation. We release our dataset for research purposes.

### Subject Apps

The 51 subject apps that formed our empirical study dataset are listed blow.

ID | Package Id | Star Num | KLOC | Category | Rating | Downloads
-- | ---------- | -------- | ---- | -------- | ------ | ---------
1 | jp.redmine.redmineclient | 56 | 19.6 | Productivity | 3.7 | 5K-10K
2 | com.duckduckgo.mobile.android | 435 | 14.9 | Tools | 4.4 | 1M-5M
3 | io.github.hidroh.materialistic | 1409 | 25.5 | News & Magazines | 4.7 | 50K-100K
4 | nya.miku.wishmaster | 82 | 54.2 | Communication | 3.6 | 100K-500K
5 | org.wikipedia | 574 | 60 | Books & Reference | 4.4 | 10M-50M
6 | aarddict.android | 72 | 4.1 | Books & Reference | 4.5 | 10K-50K
7 | acr.browser.lightning | 996 | 6 | Communication | 4.3 | 5M-10M
8 | at.tomtasche.reader | 57 | 3.9 | Business | 4 | 50K-100K
9 | au.com.wallaceit.reddinator | 29 | 13.2 | News & Magazines | 4.3 | 50K-100K
10 | ca.rmen.android.networkmonitor | 24 | 9.3 | Tools | 4.3 | 50K-100K
11 | com.adonai.manman | 18 | 6 | Education | 4.6 | 1K-5K
12 | com.cradle.iitc_mobile | 857 | 7.4 | - | - | -
13 | com.danvelazco.fbwrapper | 222 | 1.7 | Social | 4.1 | 100K-500K
14 | com.fsck.k9 | 3419 | 93.6 | Communication | 4.2 | 5M-10M
15 | com.ichi2.anki | 1010 | 51.1 | Education | 4.5 | 1M-5M
16 | com.liato.bankdroid | 251 | 17.7 | Finance | 4.1 | 100K-500K
17 | com.manuelmaly.hn | 464 | 4.3 | News & Magazines | 4.4 | 50K-100K
18 | com.newsblur | 4759 | 17.4 | News & Magazines | 3.8 | 50K-100K
19 | com.passcard | 4 | 0.2 | - | - | -
20 | com.pindroid | 247 | 7.8 | Productivity | 4.3 | 10K-50K
21 | com.shapps.mintubeapp | 210 | 2.5 | - | - | -
22 | de.danoeh.antennapod | 1699 | 47.3 | Video Players & Editors | 100K-500K
23 | de.k3b.android.locationMapViewer | 3 | 2.4 | - | - | -
24 | de.luhmer.owncloudnewsreader | 343 | 13.6 | News & Magazines | 4.5 | 1K-5K 
25 | de.ph1b.audiobook | 834 | 0.1 | Music & Audio | 4.4 | 100K-500K
26 | de.reimardoeffinger.quickdic | 59 | 5.1 | Books & Reference | 4.7 | 10K-50K
27 | de.tap.easy_xkcd | 76 | 8.7 | Comics | 4.7 | 10K-50K
28 | email.schaal.ocreader | 40 | 7.2 | - | - | -
29 | fr.gaulupeau.apps.InThePoche | 179 | 12.5 | Productivity | 4.3 | 10K-50K
30 | fr.gouv.etalab.mastodon | 11 | 24.6 | Communication | 4.5 | 5K-10K
31 | fr.renzo.wikipoff | 12 | 6.3 | - | - | -
32 | im.vector.alpha | 455 | 48.8 | Communication | 4.5 | 50K-100K
33 | in.shick.diode | 122 | 13.5 | News & Magazines | 4.4 | 10K-50K
34 | jonas.tool.saveForOffline | 71 | 2.3 | - | - | -
35 | me.ccrama.redditslide | 780 | 75.8 | News & Magazines | 4.5 | 100K-500K
36 | me.tripsit.tripmobile | 8 | 2.2 | Education | 4.7 | 10K-50K
37 | net.fred.feedex | 447 | 8.1 | News & Magazines | 4.4 | 50K-100K
38 | net.osmand.plus | 1243 | 214.8 | Maps & Navigation | 4.2 | 5M-10M
39 | nodomain.freeyourgadget.gadgetbridge | 1619 | 41.4 | - | - | -
40 | org.indywidualni.fblite | 206 | 3.6 | - | - | -
41 | org.kiwix.kiwixmobile | 100 | 82.7 | Books & Reference | 4.5 | 100K-500K
42 | org.mozilla.mozstumbler | 528 | 24.1 | Tools | 4.5 | 50K-100K
43 | org.quantumbadger.redreader | 762 | 31 | News & Magazines | 4.6 | 50K-100K
44 | org.sufficientlysecure.keychain | 904 | 76 | Communication | 4.4 | 100K-500K
45 | org.ttrssreader | 69 | 12.4 | News & Magazines | 4.3 | 10K-50K
46 | cgeo.geocaching | 808 | 78.7 | Entertainment | 4.4 | 1M-5M
47 | com.github.pockethub.android | 9156 | 20.8 | Productivity | 3.4 | 10K-50K
48 | com.linkbubble | 1043 | 23 | - | - | -
49 | org.wordpress.android | 1636 | 109.1 | Productivity | 4.2 | 5M-10M
50 | io.evercam.androidapp | 50 | 14.9 | Tools | 3.9 | 10K-50K
51 | itkach.aard2 | 142 | 4.8 | Books & Reference | 4.8 | 10K-50K

### Empirical Study Dataset
