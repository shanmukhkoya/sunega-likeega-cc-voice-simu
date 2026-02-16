# Voice Simulator - Contact Center Testing Tool

A real-time voice transcription application designed for contact center testing and training. Simulate customer-agent conversations with live speech-to-text capture, role switching, and transcript export capabilities.

## Overview

Voice Simulator lets you record and transcribe conversations between customers and agents in real-time. Perfect for contact center training, quality assurance testing, call simulation, and conversation analysis.

## Features

- **Real-time Speech Recognition** - Live voice-to-text transcription as you speak
- **Dual Role Support** - Switch between Customer and Agent roles during recording
- **Live Transcript Display** - See conversations unfold in real-time with color-coded speakers
- **Call Timer** - Track conversation duration automatically
- **Export Functionality** - Download transcripts as formatted text files
- **Clean Interface** - Modern, intuitive design with visual feedback
- **Interim Results** - See text appear as you speak, before finalization

## System Requirements

### Browser Compatibility
This application requires a browser with Web Speech API support:
- ✅ Google Chrome (recommended)
- ✅ Microsoft Edge
- ✅ Safari
- ❌ Firefox (limited support)

### Permissions Required
- Microphone access for voice recording

## Getting Started

### Installation

No installation required. Simply open the HTML file in a supported browser:

1. Download `voice-simulator-fixed-v3.html`
2. Double-click to open in your default browser
3. Grant microphone permissions when prompted

### First Time Setup

1. Open the application in Chrome, Edge, or Safari
2. You'll see a permission prompt asking for microphone access
3. Click "Allow" to grant microphone permissions
4. You're ready to start recording

## Usage Guide

### Step-by-Step: Recording Your First Conversation

#### Step 1: Start the Call
1. Look at the left panel under "Call Controls"
2. Click the green **"Start Call"** button
3. Status will change from "Inactive" to "Active" (with a green pulsing indicator)
4. Call timer starts at 0:00
5. A system message appears in the transcript: "Call initiated"

#### Step 2: Select Your Speaker Role
1. Under "Recording Controls", find the "Select Speaker" section
2. Two buttons are available:
   - **Customer** (blue) - for customer side of conversation
   - **Agent** (purple) - for agent side of conversation
3. Click **Customer** to start as the customer (default selection)
4. The selected role will be highlighted in its respective color

#### Step 3: Start Recording
1. Click the **"Start Recording"** button (cyan/blue button with microphone icon)
2. If this is your first time, browser will ask for microphone permission - click "Allow"
3. Button changes to **"Stop Recording"** (red) when active
4. You'll see "● Recording..." indicator appear in the transcript area

#### Step 4: Start Speaking
1. Speak clearly into your microphone
2. As you speak, you'll see:
   - Interim text (faded, italic) - what you're currently saying
   - Final text (solid) - confirmed transcription
3. Each finalized sentence appears as a message bubble in the transcript
4. Customer messages appear on the left (blue), Agent on the right (purple)

#### Step 5: Switch Speakers During Conversation
1. When you want to switch from Customer to Agent (or vice versa):
2. Simply click the other speaker button (Customer or Agent)
3. The new role is immediately active
4. Continue speaking - new text appears under the new role
5. No need to stop recording when switching speakers

#### Step 6: Pause Recording (Optional)
1. Click **"Stop Recording"** if you need to pause
2. Recording stops, but call remains active
3. Timer continues running
4. Click **"Start Recording"** again to resume

#### Step 7: End the Call
1. When conversation is complete, click **"End Call"** (red button)
2. Recording automatically stops
3. System message appears: "Call ended - Duration: X:XX"
4. Timer resets to 0:00
5. Transcript remains visible

#### Step 8: Export Your Transcript
1. Click the **"Export"** button (download icon)
2. A text file downloads automatically
3. Filename format: `call-transcript-[timestamp].txt`
4. File contains:
   - Header with generation date and duration
   - Full conversation with timestamps
   - Speaker labels (CUSTOMER, AGENT, SYSTEM)

### Example Conversation Flow

Here's what a typical recording session looks like:

```
[18:54:08] SYSTEM: Call initiated

[18:54:15] CUSTOMER: hello

[18:54:22] AGENT: hi how can I help you today

[18:54:37] CUSTOMER: I'm calling regarding a ticket

[18:54:44] AGENT: sure can you provide the ticket ID

[18:55:30] CUSTOMER: the ticket ID is 123698

[18:55:42] AGENT: thank you I'm looking into it right now

[18:56:44] CUSTOMER: okay that makes sense thanks for the update

[18:57:04] AGENT: thank you have a great day

[18:57:07] SYSTEM: Call ended - Duration: 2:58
```

## Interface Guide

### Left Panel - Controls

**Call Controls Section:**
- Status indicator (Active/Inactive with visual pulse)
- Call duration timer (MM:SS format)
- Start Call / End Call button

**Recording Controls Section:**
- Start Recording / Stop Recording button
- Speaker selection (Customer/Agent)
- Export button (download transcript)
- Clear button (reset transcript)

**Quick Guide:**
- Helpful tips for using the application

### Right Panel - Live Transcript

**Transcript Display:**
- Color-coded messages:
  - Blue bubbles = Customer
  - Purple bubbles = Agent
  - Gray center boxes = System messages
- Each message shows:
  - Speaker icon
  - Speaker role
  - Timestamp (HH:MM:SS)
  - Message text
- Auto-scrolls to latest message
- Shows interim text while speaking (faded/italic)

## Tips for Best Results

### Recording Quality
1. **Use a good microphone** - Built-in laptop mics work, but external mics are better
2. **Minimize background noise** - Find a quiet environment
3. **Speak clearly** - Enunciate words, don't rush
4. **Pause between sentences** - Gives the system time to finalize text
5. **Wait for finalization** - Let interim text turn solid before switching speakers

### Speaker Switching
- You can switch speakers at any time during recording
- No need to stop recording first
- Switch happens immediately
- Great for simulating back-and-forth conversations solo

### Browser Performance
- Chrome gives the best accuracy and performance
- Keep the browser tab active (don't minimize or switch tabs during recording)
- Close other unnecessary tabs to free up resources

### Troubleshooting Common Issues

**Microphone not working:**
- Check browser permissions (click lock icon in address bar)
- Try refreshing the page and allowing permissions again
- Test your mic in system settings first
- Make sure no other application is using the microphone

**Transcription is inaccurate:**
- Speak more slowly and clearly
- Reduce background noise
- Check your microphone positioning
- Try using Chrome instead of other browsers

**Recording stops automatically:**
- This is normal if there's a long pause in speech
- Just click "Start Recording" again to continue
- The auto-restart feature will handle brief pauses

**Wrong speaker label on text:**
- Make sure you selected the correct speaker before recording
- The speaker role is captured when you START speaking, not when you switch
- If needed, you can manually edit the exported transcript file

## Use Cases

### Contact Center Training
- Train new agents on call handling
- Practice different conversation scenarios
- Review and analyze conversation flow
- Create training material from real simulations

### Quality Assurance
- Test call handling procedures
- Simulate edge cases and difficult customers
- Document standard responses
- Create QA checklists from transcripts

### Product Testing
- Test voice response systems
- Validate transcription accuracy
- Stress test conversation flows
- Document test cases with actual conversations

### Documentation
- Create conversation templates
- Build FAQ responses from real calls
- Document escalation procedures
- Archive important call patterns

## File Export Format

Exported transcripts follow this format:

```
Contact Center Voice Simulation Transcript
Generated: [Date and Time]
Total Duration: [M:SS]
============================================================

[HH:MM:SS] SPEAKER: message text
[HH:MM:SS] SPEAKER: message text
...
```

## Privacy and Data

- All processing happens locally in your browser
- No data is sent to external servers
- Transcripts are only saved when you click "Export"
- Clearing your browser cache will reset all data
- No conversation history is stored between sessions

## Keyboard Shortcuts

Currently, all controls are mouse/touch-based. Keyboard shortcuts may be added in future versions.

## Known Limitations

- Requires modern browser with Web Speech API support
- Accuracy depends on speech clarity and microphone quality
- No offline mode (requires internet for speech recognition API)
- Cannot transcribe pre-recorded audio files (live speech only)
- Limited to English language (en-US)

## Future Enhancements

Potential features for future versions:
- Multi-language support
- Keyboard shortcuts
- Custom speaker labels
- Conversation analytics
- Export to different formats (JSON, CSV, PDF)
- Audio recording alongside transcription
- Sentiment analysis
- Conversation statistics

## Technical Details

### Built With
- React 18
- Web Speech API (SpeechRecognition)
- Tailwind CSS
- Vanilla JavaScript

### Browser API Used
- `SpeechRecognition` / `webkitSpeechRecognition`
- Continuous recognition with interim results
- Automatic restart on recognition end

## Support

If you encounter issues:
1. Verify browser compatibility
2. Check microphone permissions
3. Test in Chrome first
4. Clear browser cache and retry
5. Check browser console for error messages

## License

This application is provided as-is for contact center testing and training purposes.

---

**Version:** 3.0  
**Last Updated:** February 2026  
**Status:** Production Ready ✅

---

Enjoy simulating conversations and happy testing!
