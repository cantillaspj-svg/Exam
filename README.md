<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>English Teacher Certification Exam</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Custom styles for aesthetic focus and smooth transitions */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f7f9fb;
        }
        .exam-card {
            background-color: white;
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1), 0 0 10px -5px rgba(0, 0, 0, 0.04);
            transition: transform 0.3s ease-in-out;
        }
        .question-block {
            border-left: 4px solid #3b82f6; /* Blue border for visual separation */
            transition: background-color 0.2s;
        }
        .radio-option:hover {
            background-color: #eff6ff; /* Light blue on hover for clarity */
        }
        .correct-answer {
            background-color: #d1fae5; /* Green for correct */
            border-color: #10b981;
        }
        .incorrect-answer {
            background-color: #fee2e2; /* Red for incorrect */
            border-color: #ef4444;
        }
    </style>
</head>
<body class="p-4 md:p-8 min-h-screen flex items-start justify-center">

    <div class="w-full max-w-4xl">
        <header class="text-center mb-8">
            <h1 class="text-3xl font-extrabold text-blue-700">English Literature Exam: Literary Devices and Story Elements</h1>
            <p class="text-gray-600 mt-2 text-lg">For Aspiring English Teachers (Based on Course Material)</p>
            <div id="scoreDisplay" class="mt-4 p-4 text-center text-xl font-semibold rounded-lg shadow-lg hidden"></div>
        </header>

        <form id="examForm" class="space-y-8 pb-10">

            <!-- INSTRUCTIONS -->
            <div class="exam-card p-6 rounded-xl border border-blue-200">
                <h2 class="text-2xl font-bold text-blue-600 mb-3">Instructions</h2>
                <p class="text-gray-700">This exam consists of three sections: Multiple Choice, Matching, and Short Answer. Answer all questions based <strong class="font-semibold">only</strong> on the provided information. Sections 1 and 2 will be automatically graded upon submission.</p>
            </div>

            <!-- SECTION 1: MULTIPLE CHOICE -->
            <section id="mc-section" class="exam-card p-6 rounded-xl">
                <h2 class="text-2xl font-semibold text-gray-800 border-b pb-2 mb-4">Section 1: Multiple Choice (15 Points)</h2>
                <p class="text-sm text-gray-500 mb-6">Choose the best answer for each question. (1 point each)</p>

                <!-- Q1 -->
                <div class="question-block p-4 mb-4 rounded-lg bg-gray-50" data-q="mc1">
                    <p class="font-medium mb-2">1. Plot is defined as the basic sequence of events in a story. How many parts does plot have in conventional stories?</p>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc1" value="A" class="mr-2"> A. Three</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc1" value="B" class="mr-2"> B. Four</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc1" value="C" class="mr-2"> C. Five</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc1" value="D" class="mr-2"> D. Six</label>
                </div>

                <!-- Q2 -->
                <div class="question-block p-4 mb-4 rounded-lg bg-gray-50" data-q="mc2">
                    <p class="font-medium mb-2">2. What is the part of the plot that is also referred to as the **denouement**?</p>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc2" value="A" class="mr-2"> A. Exposition</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc2" value="B" class="mr-2"> B. Rising Action</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc2" value="C" class="mr-2"> C. Climax</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc2" value="D" class="mr-2"> D. Falling Action</label>
                </div>

                <!-- Q3 -->
                <div class="question-block p-4 mb-4 rounded-lg bg-gray-50" data-q="mc3">
                    <p class="font-medium mb-2">3. The **setting** of a story is defined as:</p>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc3" value="A" class="mr-2"> A. The atmosphere or feeling created by the writer.</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc3" value="B" class="mr-2"> B. The central or universal idea of a piece of fiction.</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc3" value="C" class="mr-2"> C. The time and place in which it occurs.</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc3" value="D" class="mr-2"> D. The opposition of persons or forces.</label>
                </div>

                <!-- Q4 -->
                <div class="question-block p-4 mb-4 rounded-lg bg-gray-50" data-q="mc4">
                    <p class="font-medium mb-2">4. The **mood** of a story is the atmosphere or feeling created by the writer and expressed through which other element?</p>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc4" value="A" class="mr-2"> A. Conflict</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc4" value="B" class="mr-2"> B. Theme</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc4" value="C" class="mr-2"> C. Setting</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc4" value="D" class="mr-2"> D. Dialogue</label>
                </div>

                <!-- Q5 -->
                <div class="question-block p-4 mb-4 rounded-lg bg-gray-50" data-q="mc5">
                    <p class="font-medium mb-2">5. Which of the following describes a **static character**?</p>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc5" value="A" class="mr-2"> A. A character who changes during the course of a story.</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc5" value="B" class="mr-2"> B. A well-developed character with varied traits.</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc5" value="C" class="mr-2"> C. A character who remains primarily the same during the course of a story.</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc5" value="D" class="mr-2"> D. The story's main character.</label>
                </div>

                <!-- Q6 -->
                <div class="question-block p-4 mb-4 rounded-lg bg-gray-50" data-q="mc6">
                    <p class="font-medium mb-2">6. Which type of narrator restricts their knowledge to one character’s view or behavior and uses signal pronouns such as *he*, *she*, and *they*?</p>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc6" value="A" class="mr-2"> A. Objective</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc6" value="B" class="mr-2"> B. Omniscient/third-person omniscient</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc6" value="C" class="mr-2"> C. First person/subjective</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc6" value="D" class="mr-2"> D. Omniscient/third-person limited</label>
                </div>

                <!-- Q7 -->
                <div class="question-block p-4 mb-4 rounded-lg bg-gray-50" data-q="mc7">
                    <p class="font-medium mb-2">7. A theme that is a **perception about life and the human condition** and is the central idea of a piece of fiction is also known as what type of theme?</p>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc7" value="A" class="mr-2"> A. Explicit theme</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc7" value="B" class="mr-2"> B. Universal theme</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc7" value="C" class="mr-2"> C. Limited theme</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc7" value="D" class="mr-2"> D. Subjective theme</label>
                </div>

                <!-- Q8 -->
                <div class="question-block p-4 mb-4 rounded-lg bg-gray-50" data-q="mc8">
                    <p class="font-medium mb-2">8. Which character is a **secondary character** whose main purpose is to contrast with the protagonist to highlight the main character's personality?</p>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc8" value="A" class="mr-2"> A. Antagonist</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc8" value="B" class="mr-2"> B. Flat character</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc8" value="C" class="mr-2"> C. Character Foil</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc8" value="D" class="mr-2"> D. Stock Character</label>
                </div>

                <!-- Q9 -->
                <div class="question-block p-4 mb-4 rounded-lg bg-gray-50" data-q="mc9">
                    <p class="font-medium mb-2">9. What technique involves the use of details in writing that describe what is seen, heard, smelled, tasted, or touched?</p>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc9" value="A" class="mr-2"> A. Figurative Language</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc9" value="B" class="mr-2"> B. Allusion</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc9" value="C" class="mr-2"> C. Sensory Details</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc9" value="D" class="mr-2"> D. Dialogue</label>
                </div>

                <!-- Q10 -->
                <div class="question-block p-4 mb-4 rounded-lg bg-gray-50" data-q="mc10">
                    <p class="font-medium mb-2">10. Which type of character is two-dimensional, relatively uncomplicated, and does not change throughout a story or novel?</p>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc10" value="A" class="mr-2"> A. Round character</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc10" value="B" class="mr-2"> B. Dynamic character</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc10" value="C" class="mr-2"> C. Protagonist</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc10" value="D" class="mr-2"> D. Flat character</label>
                </div>

                <!-- Q11 -->
                <div class="question-block p-4 mb-4 rounded-lg bg-gray-50" data-q="mc11">
                    <p class="font-medium mb-2">11. What is the opposition of persons or forces that brings about dramatic action central to the plot of a story?</p>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc11" value="A" class="mr-2"> A. Exposition</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc11" value="B" class="mr-2"> B. Conflict</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc11" value="C" class="mr-2"> C. Dialogue</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc11" value="D" class="mr-2"> D. Mood</label>
                </div>

                <!-- Q12 -->
                <div class="question-block p-4 mb-4 rounded-lg bg-gray-50" data-q="mc12">
                    <p class="font-medium mb-2">12. When a narrator is described as **unreliable**, what is the reader likely to do?</p>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc12" value="A" class="mr-2"> A. Accept the statements of fact without question.</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc12" value="B" class="mr-2"> B. Restrict the perspective to only one character.</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc12" value="C" class="mr-2"> C. Question or seek to qualify the statements of fact and judgment.</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc12" value="D" class="mr-2"> D. View the narrator as all-knowing.</label>
                </div>

                <!-- Q13 -->
                <div class="question-block p-4 mb-4 rounded-lg bg-gray-50" data-q="mc13">
                    <p class="font-medium mb-2">13. The lines spoken between characters in fiction or a play are called what?</p>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc13" value="A" class="mr-2"> A. Imagery</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc13" value="B" class="mr-2"> B. Sensory Details</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc13" value="C" class="mr-2"> C. Allusion</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc13" value="D" class="mr-2"> D. Dialogue</label>
                </div>

                <!-- Q14 -->
                <div class="question-block p-4 mb-4 rounded-lg bg-gray-50" data-q="mc14">
                    <p class="font-medium mb-2">14. What literary element includes the physical, psychological, cultural, or historical background against which the story takes place?</p>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc14" value="A" class="mr-2"> A. Plot</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc14" value="B" class="mr-2"> B. Setting</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc14" value="C" class="mr-2"> C. Conflict</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc14" value="D" class="mr-2"> D. Theme</label>
                </div>

                <!-- Q15 -->
                <div class="question-block p-4 mb-4 rounded-lg bg-gray-50" data-q="mc15">
                    <p class="font-medium mb-2">15. What are *he*, *she*, and *they* considered when a narrator tells a story in the third person?</p>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc15" value="A" class="mr-2"> A. Perspective markers</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc15" value="B" class="mr-2"> B. Signal pronouns</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc15" value="C" class="mr-2"> C. Subjective identifiers</label>
                    <label class="radio-option block p-2 rounded cursor-pointer"><input type="radio" name="mc15" value="D" class="mr-2"> D. Limited terms</label>
                </div>
            </section>

            <!-- SECTION 2: MATCHING -->
            <section id="matching-section" class="exam-card p-6 rounded-xl">
                <h2 class="text-2xl font-semibold text-gray-800 border-b pb-2 mb-4">Section 2: Matching (10 Points)</h2>
                <p class="text-sm text-gray-500 mb-6">Match the part of the plot (Column A) with its correct description (Column B). (2 points each)</p>

                <div class="bg-gray-100 p-4 rounded-lg mb-6">
                    <div class="grid grid-cols-2 gap-4 font-bold text-gray-700 mb-3">
                        <span>Column A (Plot Part)</span>
                        <span>Column B (Description)</span>
                    </div>
                    <ul class="space-y-2 text-sm text-gray-600">
                        <li>**A.** A series of events leading up to the climax; suspense may be present.</li>
                        <li>**B.** A series of events leading to the resolution and closure.</li>
                        <li>**C.** Tying up all the loose ends of the literature.</li>
                        <li>**D.** Introduction of characters, setting the scene (time, place, season).</li>
                        <li>**E.** The most exciting part of the plot.</li>
                    </ul>
                </div>

                <div class="space-y-4">
                    <!-- Match 1: Climax -->
                    <div class="flex items-center space-x-4 question-block p-3 rounded-lg bg-gray-50" data-q="match1">
                        <label for="match1" class="w-1/3 font-medium">1. Climax</label>
                        <select id="match1" name="match1" class="form-select w-2/3 p-2 border rounded-md shadow-sm focus:ring-blue-500 focus:border-blue-500">
                            <option value="">Select Match</option>
                            <option value="A">A</option>
                            <option value="B">B</option>
                            <option value="C">C</option>
                            <option value="D">D</option>
                            <option value="E">E</option>
                        </select>
                    </div>

                    <!-- Match 2: Exposition -->
                    <div class="flex items-center space-x-4 question-block p-3 rounded-lg bg-gray-50" data-q="match2">
                        <label for="match2" class="w-1/3 font-medium">2. Exposition</label>
                        <select id="match2" name="match2" class="form-select w-2/3 p-2 border rounded-md shadow-sm focus:ring-blue-500 focus:border-blue-500">
                            <option value="">Select Match</option>
                            <option value="A">A</option>
                            <option value="B">B</option>
                            <option value="C">C</option>
                            <option value="D">D</option>
                            <option value="E">E</option>
                        </select>
                    </div>

                    <!-- Match 3: Resolution -->
                    <div class="flex items-center space-x-4 question-block p-3 rounded-lg bg-gray-50" data-q="match3">
                        <label for="match3" class="w-1/3 font-medium">3. Resolution</label>
                        <select id="match3" name="match3" class="form-select w-2/3 p-2 border rounded-md shadow-sm focus:ring-blue-500 focus:border-blue-500">
                            <option value="">Select Match</option>
                            <option value="A">A</option>
                            <option value="B">B</option>
                            <option value="C">C</option>
                            <option value="D">D</option>
                            <option value="E">E</option>
                        </select>
                    </div>

                    <!-- Match 4: Rising Action -->
                    <div class="flex items-center space-x-4 question-block p-3 rounded-lg bg-gray-50" data-q="match4">
                        <label for="match4" class="w-1/3 font-medium">4. Rising Action</label>
                        <select id="match4" name="match4" class="form-select w-2/3 p-2 border rounded-md shadow-sm focus:ring-blue-500 focus:border-blue-500">
                            <option value="">Select Match</option>
                            <option value="A">A</option>
                            <option value="B">B</option>
                            <option value="C">C</option>
                            <option value="D">D</option>
                            <option value="E">E</option>
                        </select>
                    </div>

                    <!-- Match 5: Falling Action -->
                    <div class="flex items-center space-x-4 question-block p-3 rounded-lg bg-gray-50" data-q="match5">
                        <label for="match5" class="w-1/3 font-medium">5. Falling Action</label>
                        <select id="match5" name="match5" class="form-select w-2/3 p-2 border rounded-md shadow-sm focus:ring-blue-500 focus:border-blue-500">
                            <option value="">Select Match</option>
                            <option value="A">A</option>
                            <option value="B">B</option>
                            <option value="C">C</option>
                            <option value="D">D</option>
                            <option value="E">E</option>
                        </select>
                    </div>
                </div>
            </section>

            <!-- SECTION 3: SHORT ANSWER -->
            <section id="short-answer-section" class="exam-card p-6 rounded-xl">
                <h2 class="text-2xl font-semibold text-gray-800 border-b pb-2 mb-4">Section 3: Short Answer (Manual Grading)</h2>
                <p class="text-sm text-red-500 mb-6 font-semibold">NOTE: These answers require manual review and will not be included in the automated score.</p>

                <!-- Q1 -->
                <div class="question-block p-4 mb-4 rounded-lg bg-gray-50">
                    <p class="font-medium mb-2">1. Identify the key characteristic of an **omniscient/third-person omniscient** point of view.</p>
                    <textarea name="sa1" rows="3" class="w-full p-2 border border-gray-300 rounded-md focus:ring-blue-500 focus:border-blue-500"></textarea>
                    <div class="text-xs text-gray-500 mt-1" id="sa1_answer">
                        <!-- Answer will be revealed here -->
                    </div>
                </div>

                <!-- Q2 -->
                <div class="question-block p-4 mb-4 rounded-lg bg-gray-50">
                    <p class="font-medium mb-2">2. What is the difference between an **implicit theme** and an **explicit theme**?</p>
                    <textarea name="sa2" rows="3" class="w-full p-2 border border-gray-300 rounded-md focus:ring-blue-500 focus:border-blue-500"></textarea>
                    <div class="text-xs text-gray-500 mt-1" id="sa2_answer">
                        <!-- Answer will be revealed here -->
                    </div>
                </div>
            </section>

            <!-- SUBMIT BUTTON -->
            <div class="text-center pt-4">
                <button type="button" onclick="checkAnswers()" id="submitButton" class="bg-blue-600 hover:bg-blue-700 text-white font-bold py-3 px-8 rounded-xl shadow-lg transition duration-150 ease-in-out transform hover:scale-105">
                    Submit Exam & View Score
                </button>
            </div>
        </form>
    </div>

    <script>
        // Define the correct answers for automated grading
        const correctAnswers = {
            // Section 1: Multiple Choice (Question ID: Correct Option Letter)
            mc1: 'C', mc2: 'D', mc3: 'C', mc4: 'C', mc5: 'C', mc6: 'D', mc7: 'B', mc8: 'C',
            mc9: 'C', mc10: 'D', mc11: 'B', mc12: 'C', mc13: 'D', mc14: 'B', mc15: 'B',

            // Section 2: Matching (Question ID: Correct Description Letter)
            match1: 'E', // Climax -> E. The most exciting part of the plot.
            match2: 'D', // Exposition -> D. Introduction of characters, setting the scene (time, place, season).
            match3: 'C', // Resolution -> C. Tying up all the loose ends of the literature.
            match4: 'A', // Rising Action -> A. A series of events leading up to the climax; suspense may be present.
            match5: 'B', // Falling Action -> B. A series of events leading to the resolution and closure.
        };

        // Define the correct answers for manual review display
        const shortAnswerAnswers = {
            sa1: "The narrator tells the story in the third person from an all-knowing perspective. The knowledge is not limited by any one character’s view or behavior, as the narrator knows everything about all characters.",
            sa2: "An implicit theme is understood through inference by the reader, while an explicit theme is overtly stated by the author somewhere in the work."
        };

        function checkAnswers() {
            const form = document.getElementById('examForm');
            let score = 0;
            let totalAutoGradePoints = 25; // MC: 15 (15*1) + Matching: 10 (5*2)

            // Disable the form after submission
            const submitButton = document.getElementById('submitButton');
            submitButton.disabled = true;
            submitButton.classList.remove('hover:bg-blue-700', 'hover:scale-105');
            submitButton.classList.add('bg-gray-400');

            // --- Section 1: Multiple Choice Grading ---
            for (let i = 1; i <= 15; i++) {
                const qId = `mc${i}`;
                const correctValue = correctAnswers[qId];
                const questionBlock = document.querySelector(`[data-q="${qId}"]`);

                // Get selected answer
                const selected = form.querySelector(`input[name="${qId}"]:checked`);

                // Mark all options as disabled and check correctness
                const options = form.querySelectorAll(`input[name="${qId}"]`);
                options.forEach(option => {
                    option.disabled = true;
                    const label = option.closest('label');
                    
                    if (option.value === correctValue) {
                        // Mark the correct answer
                        label.classList.add('correct-answer');
                    }
                    
                    if (selected && option.value === selected.value) {
                        // Mark the selected answer
                        if (selected.value === correctValue) {
                            score += 1;
                        } else {
                            // Mark incorrect selection
                            label.classList.add('incorrect-answer');
                            // Ensure the correct answer is still visible if user chose wrong
                            form.querySelector(`input[name="${qId}"][value="${correctValue}"]`).closest('label').classList.add('correct-answer');
                        }
                    }
                    label.classList.remove('radio-option'); // Remove hover effect
                });
            }

            // --- Section 2: Matching Grading ---
            const matchingPoints = 2;
            for (let i = 1; i <= 5; i++) {
                const qId = `match${i}`;
                const correctValue = correctAnswers[qId];
                const selectElement = document.getElementById(qId);
                const selectedValue = selectElement.value;
                const questionBlock = document.querySelector(`[data-q="${qId}"]`);

                selectElement.disabled = true;
                selectElement.classList.remove('focus:ring-blue-500', 'focus:border-blue-500');

                // Mark question block based on correctness
                if (selectedValue === correctValue) {
                    score += matchingPoints;
                    questionBlock.classList.add('correct-answer');
                } else {
                    questionBlock.classList.add('incorrect-answer');
                }
                
                // Show correct answer in the dropdown's display
                const correctMatchText = document.createElement('span');
                correctMatchText.className = 'ml-4 text-xs font-semibold';
                correctMatchText.textContent = `Correct Match: ${correctValue}`;
                questionBlock.appendChild(correctMatchText);
            }

            // --- Section 3: Short Answer Display ---
            document.getElementById('sa1_answer').innerHTML = `<strong class="text-blue-600">Expected Answer:</strong> ${shortAnswerAnswers.sa1}`;
            document.getElementById('sa2_answer').innerHTML = `<strong class="text-blue-600">Expected Answer:</strong> ${shortAnswerAnswers.sa2}`;


            // --- Final Score Display ---
            const percentage = ((score / totalAutoGradePoints) * 100).toFixed(1);
            const scoreDisplay = document.getElementById('scoreDisplay');
            
            scoreDisplay.innerHTML = `
                <p class="text-green-700">Automated Grade Complete!</p>
                <p class="mt-2 text-2xl font-extrabold">Score: <span class="text-blue-700">${score}</span> / ${totalAutoGradePoints} Points</p>
                <p class="text-base text-gray-500">Percentage: ${percentage}%</p>
                <p class="text-sm mt-3 text-red-600">Note: Sections 1 & 2 are graded. Short Answer section requires manual review.</p>
            `;
            scoreDisplay.classList.remove('hidden');
            scoreDisplay.scrollIntoView({ behavior: 'smooth', block: 'start' });
        }
    </script>
</body>
</html>
