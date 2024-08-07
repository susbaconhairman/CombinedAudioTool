# CombinedAudioTool
- A Tool for CombinedAudio.bin for Minecraft for New Nintendo 3DS Edition (MC3DS) with a plethora of Features.
- Only support Windows Platforms Officially, due to being built and made using some Windows API functions.

## Feature Set:
- Extract All FSB Soundbank Files in the Archive.
- Extract a FSB Soundbank File by Name/Sound-ID.
- Get File name(s) from Soundbank Files for easier recognition.
- Rename Extracted files to original filename(s).
- Rebuild `CombinedAudio.bin` with new Custom Audio Files.
- Extract Header from `CombinedAudio.bin`.
- Add padding to files automatically (Requires Original Extracted File).
- Collect all Sound Names/ID's.
- Rename all Segments to Original Filenames.
- Grab Segment File Sizes individually, or altogether.
- Updating your Script as new features become avaliable.
- Extract Audio from FSB Files (now including GCADPCM FSB Soundbank Files).
- Convert `*.wav` back into GCADPCM/DSADPCM.
- Restore CATool File Integrity.
- Encode Minecraft 3DS Music Files from Wave Files.
- Convert any Audio Filetype to Wave (requires FFMPEG).
- Install FFMPEG via Command Line.
- Add your own Custom Audio/Ambience/SFX to Minecraft 3DS.

## Download(s):
- Download [Here](https://github.com/Minecraft-3DS-Community/CombinedAudioTool/releases/download/v2.0/CATool.zip).
- Requires `Python 3.8+` and `Python STD` (Installed alongside Python).

## Usage:
```
python CATool.py
       --eca,  extract-ca     [CombinedAudioPATH]                            > Extracts All FSB Soundbank Files from the CombinedAudio.bin Archive.
       --fn,   find-sn        [SegmentFilePATH]                              > Find the Segment Name from an Extracted FSB Soundbank File via --eca Flag.
       --rs,   rename-s       [SegmentFilePATH]                              > Rename a Segment File FSB Soundbank File back to it's Original Filename.
       --gh,   get-header     [CombinedAudioPATH]                            > Extracts the Header from the CombinedAudio.bin Archive.
       --rca,  rebuild-ca     [SegmentOutFolderPATH]                         > Rebuilds the CombinedAudio.bin Archive via Segment Files.
       --ap,   add-padding    [OriginalFilePATH]       [ModifiedFilePATH]    > Adds padding to set the Modified File Equal to the Original File Size.
       --ne,   name-extract   [CombinedAudioPATH]      [Sound Name/ID]       > Extracts a FSB Soundbank File from the CombinedAudio.bin Archive via Name/SoundID.
       --ra,   rename-all     [SegmentFolderPATH]                            > Renames all Segment Files back to their original FSB Soundbank Filename(s).
       --gsid, get-soundid    [CombinedAudioPATH]                            > Gets all Sound Names/ID's and Dumps them to a *.txt File.
       --gssg, get-size-seg   [SegmentFilePATH]                              > Gets the size of a specific Segment Soundbank FSB File.
       --gs,   get-size       [SegmentOutFolderPATH]                         > Gets the size of all Segment Soundbank FSB Files.
       --exa,  extract-seg    [SegmentFilePATH]                              > Attempts to extract Audio from Segment Soundbank FSB Files.
       --cwav, convert-wave   [SegmentFilePATH]        [FileToConvertPATH]   > Convert Custom Audio to Nintendo 'GCADPCM'/'DSADPCM' Format (*.dsp).
       --pa,   play-audio     [WaveFilePATH]                                 > Play Audio from a Wave-File.
       --gmsc, generate-music [WaveFilePATH]                                 > Generates a Valid Music FSB Soundbank File for Minecraft 3DS Edition from a Wave File.
       --atw,  to-wave        [AudioFileToConvertToWavPATH]                  > Convert basically any Audio format like *.ogg or *.mp3 to Wave Format.
       --impg, inst-ffmpeg                                                   > Install FFMPEG to '.\extrcd\mpg\bin'.
       --efrw, ext-fsb-raw    [SegmentFilePATH]                              > Extracts the raw GCADPCM/DSPADPCM Audio from an *.fsb Soundbank File.
       --edrw, ext-dsp-raw    [GeneratedDspFilePATH]                         > Extracts the raw GCADPCM/DSPADPCM Audio from a Nintendo *.dsp Audio File.
       --rsnd, replace-snd    [SegmentFilePATH]        [DspFilePATH]         > Convert Nintendo *.dsp Audio File to *.fsb Soundbank File.
       --upd,  update                                                        > Updates From Current Version to the Latest Version of 'CATool.py'.
       --rstr, restore                                                       > Basically an Emergancy Version of '--upd' that Wipes all Files from CATool and Reinstalls them.
       --h,    help                                                          > Displays this Message.
```
### Help Message:
```
python CATool.py --h
```
![image](https://github.com/Minecraft-3DS-Community/CombinedAudioTool/assets/78656905/7d2d4adb-6f45-4484-85ee-c519ad9058b7)

## Sound ID's
```
1 thunder1
2 thunder2
3 explode1
4 explode2
5 rain1
6 rain2
7 shimmerblock
8 fire_crackle2
9 add_item1
10 add_item2
11 add_item3
12 break1
13 break2
14 place1
15 place2
16 remove_item1
17 remove_item2
18 rotate_item1
19 rotate_item2
20 death1
21 death3
22 grow1
23 grow4
24 empty_lava1
25 empty_lava2
26 empty1
27 empty2
28 fill_lava1
29 fill_lava2
30 fill1
31 fill2
32 splash
33 fallbig
34 fallsmall
35 weak1
36 weak2
37 weak3
38 hit1
39 hit2
40 hit3
41 cloth1
42 cloth2
43 cloth3
44 grass1
45 grass2
46 grass3
47 gravel1
48 gravel2
49 gravel3
50 sand1
51 sand2
52 sand3
53 snow1
54 snow2
55 snow3
56 stone1
57 stone2
58 stone3
59 wood1
60 wood2
61 wood3
62 in
63 out
64 fire
65 ignite
66 lava
67 lavapop
68 water
69 base
70 death
71 hurt1
72 hurt2
73 hurt3
74 idle1
75 idle2
76 idle3
77 takeoff
78 breathe1
79 breathe2
80 death
81 hit1
82 hit2
83 hit3
84 fireball4
85 hurt1
86 hurt2
87 plop
88 say1
89 say2
90 say3
91 step1
92 step2
93 hurt1
94 hurt2
95 hurt3
96 say1
97 say2
98 say3
99 step1
100 step2
101 step3
102 milk1
103 death
104 say1
105 say2
106 say3
107 death
108 hit1
109 hit2
110 hit3
111 idle1
112 idle2
113 idle3
114 portal
115 portal2
116 scream1
117 scream2
118 scream3
119 stare
120 hit1
121 hit2
122 wings1
123 wings3
124 wings5
125 growl2
126 growl3
127 affectionate_scream
128 charge
129 death
130 moan1
131 moan2
132 moan3
133 scream1
134 scream2
135 scream3
136 ambient1
137 attack_loop
138 curse
139 elder_death
140 elder_hit1
141 elder_idle3
142 flop1
143 guardian_death
144 guardian_hit1
145 land_death
146 land_hit1
147 land_idle1
148 angry1
149 death1
150 death2
151 idle1
152 idle2
153 idle3
154 idle4
155 idle5
156 spit1
157 spit2
158 hurt1
159 hurt2
160 hurt3
161 eat1
162 eat2
163 eat3
164 step1
165 step2
166 step3
167 step4
168 step5
169 swag
170 angry1
171 armor
172 breathe1
173 breathe2
174 breathe3
175 death
176 angry1
177 angry2
178 death
179 hit1
180 hit2
181 hit3
182 idle1
183 idle2
184 idle3
185 eat1
186 eat2
187 eat3
188 gallop1
189 gallop2
190 gallop3
191 hit1
192 hit2
193 hit3
194 idle1
195 idle2
196 idle3
197 jump
198 land
199 leather
200 death
201 hit1
202 hit2
203 hit3
204 idle1
205 idle2
206 idle3
207 soft1
208 soft2
209 soft3
210 wood1
211 wood2
212 wood3
213 death
214 hit1
215 hit2
216 hit3
217 idle1
218 idle2
219 idle3
220 idle2
221 death1
222 hurt2
223 step4
224 throw
225 death
226 hit1
227 hit2
228 hit3
229 walk1
230 walk2
231 walk3
232 ambient1
233 ambient2
234 ambient5
235 close1
236 close3
237 death1
238 death2
239 hurt_close1
240 hurt_close2
241 hurt1
242 hurt2
243 hurt3
244 open2
245 open3
246 shoot1
247 shoot4
248 hit1
249 hit2
250 hit3
251 big1
252 big2
253 big3
254 jump1
255 jump2
256 jump3
257 small1
258 small2
259 small3
260 death
261 pig_boost
262 pig_boost
263 pig_boost
264 say1
265 say2
266 say3
267 step1
268 step2
269 step3
270 hurt1
271 hurt2
272 hurt3
273 hurt4
274 idle2
275 idle3
276 hop1
277 hop2
278 hop3
279 bunnymurder
280 say1
281 say2
282 say3
283 shear
284 step1
285 step2
286 step3
287 hit2
288 hit3
289 kill
290 say1
291 say2
292 say3
293 step1
294 step2
295 step3
296 death
297 hurt1
298 hurt2
299 hurt3
300 say1
301 say2
302 say3
303 step1
304 step2
305 step3
306 big1
307 big2
308 big3
309 small1
310 small2
311 small3
312 attack1
313 attack2
314 death1
315 death2
316 death3
317 hurt1
318 hurt2
319 hurt3
320 bow
321 death
322 say1
323 say2
324 say3
325 step1
326 step2
327 step3
328 ambient1
329 ambient2
330 death3
331 hurt1
332 hurt2
333 idle2
334 death1
335 hurt4
336 step3
337 death
338 haggle1
339 haggle3
340 hit1
341 hit2
342 hit3
343 idle1
344 idle2
345 idle3
346 no1
347 no2
348 yes1
349 yes2
350 death1
351 death2
352 hurt1
353 hurt2
354 hurt3
355 idle1
356 idle2
357 idle3
358 fangs
359 idle1
360 idle2
361 idle3
362 cast1
363 cast2
364 death1
365 death2
366 hurt1
367 hurt2
368 prepare_attack1
369 prepare_attack2
370 prepare_summon
371 prepare_wololo
372 idle1
373 idle2
374 death1
375 death2
376 hurt1
377 hurt2
378 charge1
379 charge2
380 ambient5
381 ambient1
382 ambient2
383 death1
384 death2
385 death3
386 hurt1
387 hurt2
388 hurt3
389 drink1
390 drink2
391 drink3
392 throw1
393 throw2
394 throw3
395 idle1
396 woodbreak
397 death
398 death1
399 shoot
400 spawn
401 bark1
402 bark2
403 bark3
404 death
405 growl1
406 growl2
407 hurt1
408 hurt2
409 hurt3
410 panting
411 shake
412 step1
413 step2
414 step3
415 whine
416 hiss1
417 hiss2
418 hitt1
419 hitt2
420 hitt3
421 meow1
422 meow2
423 meow3
424 purr1
425 purr2
426 purreow1
427 purreow2
428 idle1
429 idle4
430 idle1
431 idle2
432 step1
433 step2
434 warning1
435 warning2
436 hurt1
437 hurt2
438 death1
439 death2
440 death
441 hurt1
442 hurt2
443 remedy
444 unfect
445 say1
446 say2
447 step1
448 step2
449 step3
450 wood1
451 wood2
452 wood3
453 zpig1
454 zpig2
455 zpig3
456 zpigangry1
457 zpigangry2
458 zpigangry3
459 zpigdeath
460 zpighurt1
461 zpighurt2
462 say1
463 say2
464 say3
465 death
466 hurt1
467 hurt2
468 bass
469 bassattack
470 bd
471 harp
472 hat
473 pling
474 snare
475 portal
476 anvil_break
477 anvil_land
478 anvil_use
479 bowhit1
480 bowhit2
481 bowhit3
482 break
483 burp
484 chestclosed
485 chestopen
486 close
487 open
488 click
489 door_close
490 door_open
491 drink
492 eat1
493 eat2
494 eat3
495 fizz
496 fuse
497 glass1
498 glass2
499 glass3
500 levelup
501 orb
502 pop
503 pop2
504 swim1
505 swim3
506 swim4
507 hurt
508 toast
509 use_totem
510 camera1
511 camera2
512 camera3
513 ladder1
514 ladder2
515 ladder3
516 cloth1
517 cloth2
518 cloth3
519 grass1
520 grass2
521 grass3
522 gravel1
523 gravel2
524 gravel3
525 sand1
526 sand2
527 sand3
528 snow1
529 snow2
530 snow3
531 stone1
532 stone2
533 stone3
534 wood1
535 wood2
536 wood3
537 cloth1
538 cloth2
539 cloth3
540 grass1
541 grass2
542 grass3
543 gravel1
544 gravel2
545 gravel3
546 sand1
547 sand2
548 sand3
549 snow1
550 snow2
551 snow3
552 stone1
553 stone2
554 stone3
555 wood1
556 wood2
557 wood3
```
