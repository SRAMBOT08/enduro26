# Engine Sound Setup for ENDURO'26

## Required Sound Files

To enable engine sounds on your website, you need to add 3 audio files to the project directory:

### 1. **engine-start.mp3**
- Engine ignition/startup sound
- Duration: 1-2 seconds
- Plays once when the ignition button is clicked

### 2. **engine-idle.mp3**
- Low RPM engine idle sound
- Should be a **looping** sound (seamless loop)
- Duration: 2-5 seconds
- Plays continuously at low RPM

### 3. **engine-rev.mp3**
- High RPM engine revving sound
- Should be a **looping** sound (seamless loop)
- Duration: 2-5 seconds
- Pitch automatically adjusts based on RPM (0.8x to 2x speed)

## Where to Find Engine Sounds

### Free Sound Resources:
1. **Freesound.org** - https://freesound.org/
   - Search: "motorcycle engine", "dirt bike", "engine start"
   
2. **Pixabay** - https://pixabay.com/sound-effects/search/engine/
   - Free sound effects, no attribution required
   
3. **YouTube Audio Library** - Convert to MP3
   - Search for engine sounds

4. **Mixkit** - https://mixkit.co/free-sound-effects/engine/
   - Free sound effects

### Recommended Search Terms:
- "motorcycle engine idle"
- "dirt bike rev"
- "motocross engine"
- "engine startup"
- "motorcycle throttle"

## How Sounds Work

- **Engine Start**: Plays when you click the ignition button
- **Idle Sound**: Plays continuously at low RPM (< 500 RPM)
- **Rev Sound**: 
  - Volume increases with RPM
  - Pitch increases automatically (using playback rate)
  - Fades in as you throttle up
  - Fades out when you release the throttle

## Testing Without Sound Files

The website will still work without the sound files - it just won't play audio. The browser console may show errors about missing audio files, but all visual features will function normally.

## File Format Support

- **Recommended**: MP3 format (.mp3)
- **Alternative**: WAV format (.wav) - larger file size
- **Modern browsers**: Also support .ogg and .m4a

## Volume Levels

Current volume settings in the code:
- Engine Start: 80%
- Engine Idle: 60%
- Engine Rev: 0-80% (increases with RPM)

You can adjust these in the JavaScript if needed.
