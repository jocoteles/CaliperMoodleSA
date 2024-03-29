[![DOI](https://zenodo.org/badge/476100745.svg)](https://zenodo.org/badge/latestdoi/476100745)

**CaliperMoodleSA** - Moodle Short Answers question generator for Caliper
==============

This is a Moodle Short Answer question generator with the objective of teaching and evaluating the learning of the Caliper measurement instrument. The question generator consists of a [configuration page](https://jocoteles.github.io/CaliperMoodleSA/) that allows you to create a bank of random questions that are exported to a single file in Moodle XML format. This file can be uploaded into a Moodle course and incorporated into a Quiz Activity as a random question. Each question corresponds to a type of caliper drawn at random and with a random opening. Configuration items are as follows:

- *Question text*. Text that will accompany the image of the caliper drawn in the question. It may contain instructions on how to enlarge and pan the image in order to make the instrument easier to read. This text is identical for all drawn questions.
- *Types of caliper to be included in the questions*. Allows you to choose which types of calipers to be included in the drawing of questions (Verniers with 5, 10, 20 and 50 divisions).
- *Number of random questions*. The number of random questions to include in the Moodle XML file. A high number is indicated for different students to receive different questions or for the same student to have a reduced chance of receiving a repeated question in a Quiz Activity with multiple caliper questions.
- *Decimal separators accepted*. The type of decimal separator accepted in the student's answer can be chosen as dot and/or comma. This option is associated with the regulation of each country and the teacher's choice to make this regulation more flexible or not in the response.
- *Penalty for each wrong attempt*. Penalty for each attempt to answer the randomly selected question, ranging from 0 to 1, where 1 corresponds to 100% of the value of the question. That is, when the student makes a mistake and tries to answer it again, the value of the question is subtracted by this penalty.
- *Generate Moodle XML file*. By clicking on this button, the Moodle XML file is generated and a window for saving the file on the computer is opened to the user.
- *Render a new sample*. Button used to render the image of a caliper sample according to the chosen settings. When clicking this button, in addition to the image of a new caliper sample, the value of the corresponding expected reading is also shown. This sample is only intended to provide an example of the type of caliper that will be included in the Moodle XML file.

After saving the Moodle XML file on the computer, the teacher (or course manager) must log in to the corresponding Moodle course and access the Question Bank available in Course Administration. There, a category of questions must be created that will receive the questions from the caliper. Then, import it to the created category by selecting the option for *Moodle XML file format* and uploading the file saved on the computer. With this, the questions can be used in a Quiz Activity by adding a random question chosen from the created category.

This project uses the Javascript libraries [svg-pan-zoom](https://github.com/bumbu/svg-pan-zoom), [hammerjs](https://github.com/hammerjs/hammer.js) and [FileSaver.js](https://github.com/eligrey/FileSaver.js/).

The Caliper svg parts were adapted from [Caliper Wikipedia](https://en.wikipedia.org/wiki/File:Vernier_caliper.svg).
