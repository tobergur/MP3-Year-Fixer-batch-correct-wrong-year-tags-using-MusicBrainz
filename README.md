# MP3-Year-Fixer-batch-correct-wrong-year-tags-using-MusicBrainz
I had 854 MP3s with wrong year tags and didn't want to fix them one by one so I had Claude write me a script. im ashamed ik, but it works

It reads each MP3's artist, title, and album tags, looks up the correct year on MusicBrainz, and writes it back and only editing the year field. It matches on all three fields to avoid getting confused by songs with the same title, and pulls from the original recording date so you don't get remaster years.

Not perfect though. some songs it can't find, and occasionally it still writes a wrong year. It logs everything to a .txt file so you can fix stragglers manually.

Requires mutagen and musicbrainzngs (pip install mutagen musicbrainzngs). Change the FOLDER path at the top to yours and run it. ~15 min for 850 files due to MusicBrainz's rate limit.

i am not a coder; this was AI-generated. If you're a real dev and want to make a better version, please do and share!!!
