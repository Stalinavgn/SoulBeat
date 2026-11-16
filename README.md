♥ SoulBeat
A visual, no-code editor for UNDERTALE / DELTARUNE-style bullet fights synced to music. Drop a track, place attack blocks on the beat grid, watch the fight instantly — then export a ready mod for Create Your Frisk or record a video right in the browser.

▶ Open the editor: https://stalinavgn.github.io/soulbeat/

No install, no account, no coding. One HTML file that also works offline.

What it does
Music first. Load mp3 / wav / ogg — tempo and first beat are detected, the waveform and beat grid appear on the timeline. Tap tempo and a metronome are there if the detection misses.
16 attack blocks. Ring, spiral, aimed shot, rain, wall with a gap, bones, laser, spinning cross, snake, chasers, fountain, flash mines — plus four Deltarune-style traps: closing cage, spinning scythes, egg bombs and cross slash.
Everything is a slider. Every block has a "Rhythm" (every beat, half beat, triplets…), bullet type (white / cyan / orange / green / decor), colour and size. The preview updates as you drag.
26 built-in bullet symbols in themed sets: Classic, Dark world, RoboPunk, AngelPunk, MedievalPunk, FuturePunk, HellPunk, DruidPunk. Or use your own PNG.
Enemy above the arena. PNG, GIF or video (with optional green-screen removal). Drag it into place with the mouse.
Stage control. Resize and move the arena, recolour it, flash and shake the screen, play sounds, switch to the blue soul with gravity.
Made for video. Chroma-key backgrounds, hidden interface, immortal mode, "start on Z", and a recorded take that replays your exact dodging path.
Two ways out. To game writes a complete Create Your Frisk mod (Lua + sprites + music). Video records the preview to .webm with sound.
English and Russian interface, switchable at any time.
Quick start
Open the editor (link above) in Chrome or Edge.
Drag a music file into the window.
Click an attack on the left — it lands on the red line. Drag it, stretch it, tune it on the right.
Press Space to play.
Press To game and pick your Create Your Frisk folder (or download a ZIP and unpack it into Mods). Start CYF and choose the mod named SoulBeat <your title>.
Your work is saved automatically in the browser. Use Project → Save to file to keep a copy or move it to another computer.

Keys
Key	Action
Space	play / pause
Enter	drop the chosen block at the playhead (works while the music plays)
Delete	delete selected blocks
Ctrl+D / Ctrl+C / Ctrl+V	duplicate / copy / paste
Ctrl+Z / Ctrl+Y	undo / redo
L	loop the selected block
M	metronome
Alt while dragging	no snapping
Ctrl + wheel	timeline zoom
Good to know
Writing straight into the game folder needs a Chromium browser (Chrome, Edge). In other browsers use the ZIP export.
GIF and video enemies are turned into frames: up to 240 frames, longest side 256 px, videos are cut to their first 20 seconds and their sound is not used.
The recorded video shows the editor preview. Fonts and buttons differ slightly from the real game — for the true in-game look, export to CYF and capture the screen.
The exported Lua runtime is checked frame-by-frame against the editor preview with a simulated CYF API ("Chasers" may drift slightly because they steer in real time). Reports from the real engine are welcome — please open an issue with the error text or a screenshot.
Not included yet: monster dialogue bubbles and FIGHT / ACT turn logic. The export is one continuous music-driven wave.
Build from source
The editor is plain JavaScript without dependencies. index.html is assembled from the files in src/:

node build.js
File	What is inside
src/engine.js	attack library, baking blocks into bullets, the simulator
src/runtime.lua	the same simulator for Create Your Frisk
src/export.js	Lua generation, ZIP and WAV writers
src/app1.js – app3.js	interface: preview, timeline, panels, import and export
src/i18n_*.js	Russian dictionary (English is the source language)
Support
If SoulBeat saved you an evening, you can support the author. More projects: github.com/Stalinavgn.

Disclaimer
SoulBeat is a free fan-made tool. It is not affiliated with or endorsed by Toby Fox, UNDERTALE, DELTARUNE or the Create Your Frisk team. UNDERTALE and DELTARUNE belong to their owners. SoulBeat ships no game assets: all built-in sprites are drawn by the editor itself.

Licensed under the MIT License.

По-русски
SoulBeat — визуальный редактор боёв в стиле UNDERTALE / DELTARUNE под музыку, без программирования.

▶ Открыть редактор: https://stalinavgn.github.io/soulbeat/ (язык переключается кнопкой EN / RU вверху).

Открой редактор в Chrome или Edge и перетащи в окно трек.
Кликай по атакам слева — они встают на красную линию. Двигай их мышкой, настраивай ползунками справа.
Пробел — смотреть бой под музыку.
«В игру» собирает готовый мод для Create Your Frisk, «Видео» записывает ролик прямо из браузера.
Внутри: 16 атак (включая четыре ловушки в духе Deltarune), 26 символов-пуль в тематических наборах, враг из PNG / GIF / видео, управление ареной, хромакей-фон, запись дубля и метроном.

Поддержать автора: DonationAlerts.
