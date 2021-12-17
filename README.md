# OMR_Reader
## What is Optical Mark Recognition (OMR)
Optical Mark Recognition, or OMR for short, is the process of automatically analyzing human-marked documents and interpreting their results.

Arguably, the most famous, easily recognizable form of OMR are bubble sheet multiple choice tests. If you’re unfamiliar with “bubble sheet tests” or the trademark/corporate name of “Scantron tests”, they are simply multiple-choice tests that you take as a student. Each question on the exam is a multiple choice — and you use a #2 pencil to mark the “bubble” that corresponds to the correct answer.

In short, what I’m trying to say is that there is a massive market for Optical Mark Recognition and the ability to grade and interpret human-marked forms and exams.
## Implementing a bubble sheet scanner and grader using OMR, Python, and OpenCV

Below I have included an example filled in bubble sheet exam that I have put together for this project:

![omr_test_01](https://user-images.githubusercontent.com/56927015/146536738-448b877a-9092-474c-8627-a615bad5da97.png "omr_test_01")

We’ll be using this as our example image as we work through the steps of building our test grader.

## The 7 steps to build a bubble sheet scanner and grader
The goal is to build a bubble sheet scanner and test grader using Python and OpenCV.

To accomplish this, our implementation will need to satisfy the following 7 steps:

* Step #1: Detect the exam in an image.
* Step #2: Apply a perspective transform to extract the top-down, birds-eye-view of the exam.
* Step #3: Extract the set of bubbles (i.e., the possible answer choices) from the perspective transformed exam.
* Step #4: Sort the questions/bubbles into rows.
* Step #5: Determine the marked (i.e., “bubbled in”) answer for each row.
* Step #6: Lookup the correct answer in our answer key to determine if the user was correct in their choice.
* Step #7: Repeat for all questions in the exam.

## Prerequisites

We would require the following python libraries to make this program: 
* numpy
* argparse (*optional*)
* imutils
* cv2

## Credits
This **OMR Reader** is an implementation of the original [**Bubble sheet multiple choice scanner and test grader using OMR, Python, and OpenCV**](https://www.pyimagesearch.com/2016/10/03/bubble-sheet-multiple-choice-scanner-and-test-grader-using-omr-python-and-opencv/) by [PyImageSearch.com](www.pyimagesearch.com).
