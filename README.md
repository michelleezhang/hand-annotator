# hand annotator
This is a tool for interactive text annotation based on hand gesture recognition. The primary goal of this tool is to provide an accessible and cost-effective solution for annotating text in videos, catering to the increasing demand for interactive digital learning tools in an evolving educational landscape.

Users can record a video of themselves with a piece of text and perform certain hand gestures to select areas of the text and annotate them.
The hand annotator recognizes five gestures:
- Open palm: start or stop text selection
- Thumbs up:  select text
- Victory sign: highlight selected text
- Love sign: change color of selected text
- Closed fist: erase highlights or color changes in the currently selected text
The program will generate an output video with the identified annotations applied.

This implementation uses the Google MediaPipe library for gesture recognition, employing a two step neural network pipeline to identify hand landmarks in a given video frame.

The program operates under the simplifying assumptions of a stationary camera frame, text aligned with the screen, and only one hand present in a given frame.
