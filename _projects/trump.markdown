---
layout: page
title: Donald Trump Deepfake
description: Can you spot the audio TrumpFake?
img: https://upload.wikimedia.org/wikipedia/commons/thumb/5/56/Donald_Trump_official_portrait.jpg/440px-Donald_Trump_official_portrait.jpg
importance: 3
category: demos
---

<style>
    /* Styling the table */
table {
    width: 100%;
    border-collapse: collapse;
    margin: 20px 0;
    font-family: Arial, sans-serif;
}



/* Styling the table cells */
td {
    padding: 10px 15px;
    border: 1px solid #e0e0e0;
}

/* Styling the button */
button {
    padding: 5px 15px;
    border: none;
    background-color: #007BFF;
    color: #fff;
    cursor: pointer;
    transition: background-color 0.3s;
}

/* Button hover effect */
button:hover {
    background-color: #0056b3;
}

</style>

<p>
    Listen to the following audio samples of Donald Trump, the 45th president of the United States.
    Some are fake, some are authentic. Can you identify the deepfakes?
</p>

<div class="row">
    <div class="col text-center">
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/56/Donald_Trump_official_portrait.jpg/440px-Donald_Trump_official_portrait.jpg" class="center-block" alt="Responsive image"
             style="max-width: 50%">
    </div>
</div>

<table>
    <thead>
        <tr>
            <th scope="col">#</th>
            <th scope="col">Audio</th>
            <th scope="col">Fake or Authentic?</th>
            <th scope="col">Solution</th>
        </tr>
    </thead>
    <tbody>
        <!-- Sample 0 -->
        <tr>
            <th scope="row">0</th>
            <td><audio controls src="/assets/wav/trump_samples/0.wav"></audio></td>
            <td><button onclick="toggleSolution('solution_0')">Show solution</button></td>
            <td><div id="solution_0" style="display:none;">Fake</div></td>
        </tr>
        <!-- Sample 1 -->
        <tr>
            <th scope="row">1</th>
            <td><audio controls src="/assets/wav/trump_samples/1.wav"></audio></td>
            <td><button onclick="toggleSolution('solution_1')">Show solution</button></td>
            <td><div id="solution_1" style="display:none;">True</div></td>
        </tr>
        <!-- Sample 2 -->
        <tr>
            <th scope="row">2</th>
            <td><audio controls src="/assets/wav/trump_samples/2.wav"></audio></td>
            <td><button onclick="toggleSolution('solution_2')">Show solution</button></td>
            <td><div id="solution_2" style="display:none;">Fake</div></td>
        </tr>
        <!-- Sample 3 -->
        <tr>
            <th scope="row">3</th>
            <td><audio controls src="/assets/wav/trump_samples/3.wav"></audio></td>
            <td><button onclick="toggleSolution('solution_3')">Show solution</button></td>
            <td><div id="solution_3" style="display:none;">Fake</div></td>
        </tr>
        <!-- Sample 4 -->
        <tr>
            <th scope="row">4</th>
            <td><audio controls src="/assets/wav/trump_samples/4.wav"></audio></td>
            <td><button onclick="toggleSolution('solution_4')">Show solution</button></td>
            <td><div id="solution_4" style="display:none;">True</div></td>
        </tr>
        <!-- Sample 5 -->
        <tr>
            <th scope="row">5</th>
            <td><audio controls src="/assets/wav/trump_samples/5.wav"></audio></td>
            <td><button onclick="toggleSolution('solution_5')">Show solution</button></td>
            <td><div id="solution_5" style="display:none;">Fake</div></td>
        </tr>
        <!-- Sample 6 -->
        <tr>
            <th scope="row">6</th>
            <td><audio controls src="/assets/wav/trump_samples/6.wav"></audio></td>
            <td><button onclick="toggleSolution('solution_6')">Show solution</button></td>
            <td><div id="solution_6" style="display:none;">Fake</div></td>
        </tr>
        <!-- Sample 7 -->
        <tr>
            <th scope="row">7</th>
            <td><audio controls src="/assets/wav/trump_samples/7.wav"></audio></td>
            <td><button onclick="toggleSolution('solution_7')">Show solution</button></td>
            <td><div id="solution_7" style="display:none;">Fake</div></td>
        </tr>
        <!-- Sample 8 -->
        <tr>
            <th scope="row">8</th>
            <td><audio controls src="/assets/wav/trump_samples/8.wav"></audio></td>
            <td><button onclick="toggleSolution('solution_8')">Show solution</button></td>
            <td><div id="solution_8" style="display:none;">True</div></td>
        </tr>
        <!-- Sample 9 -->
        <tr>
            <th scope="row">9</th>
            <td><audio controls src="/assets/wav/trump_samples/9.wav"></audio></td>
            <td><button onclick="toggleSolution('solution_9')">Show solution</button></td>
            <td><div id="solution_9" style="display:none;">True</div></td>
        </tr>
    </tbody>
</table>

<script>
function toggleSolution(id) {
    var element = document.getElementById(id);
    if (element.style.display === "none") {
        element.style.display = "block";
    } else {
        element.style.display = "none";
    }
}
</script>