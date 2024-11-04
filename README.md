<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Onboarding Checklist</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #ffffff;
            color: #333333;
            margin: 0;
            padding: 0;
        }
        .container {
            max-width: 800px;
            margin: 20px auto;
            padding: 20px;
            border: 1px solid #ddd;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            background-color: #f9f9f9;
        }
        h1 {
            color: #ff7f00;
            font-size: 2em;
            margin-bottom: 5px;
        }
        h2 {
            color: #ff7f00;
            font-size: 1.5em;
            margin-bottom: 20px;
        }
        .section {
            margin-top: 20px;
        }
        .section h3 {
            color: #333333;
            font-size: 1.2em;
            margin-bottom: 10px;
        }
        .section ul {
            list-style-type: none;
            padding: 0;
        }
        .section li {
            padding: 10px;
            margin-bottom: 10px;
            border-radius: 5px;
            background-color: #ffffff;
            border: 1px solid #ddd;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            display: flex;
            align-items: center;
        }
        .section li input[type="checkbox"] {
            margin-right: 10px;
            transform: scale(1.2);
        }
        .reset-button {
            background-color: #ff7f00;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            margin-top: 20px;
            display: block;
            width: 100%;
            max-width: 200px;
            margin-left: auto;
            margin-right: auto;
        }
        .reset-button:hover {
            background-color: #e66e00;
        }
    </style>
</head>
<body>

<div class="container">
    <h1>Onboarding Checklist</h1>
    <h2>Streamline Your Onboarding</h2>

    <div class="section">
        <h3>Master Schedule Review</h3>
        <ul>
            <li><input type="checkbox"> Review the daily master schedule for assigned tasks and confirm details with the producer before proceeding.</li>
        </ul>
    </div>

    <div class="section">
        <h3>Setup & Tools</h3>
        <ul>
            <li><input type="checkbox"> Install Google Drive for Desktop: Settings > Get Drive for desktop.</li>
            <li><input type="checkbox"> Use Google Drive App for offline media and opening applications.</li>
            <li><input type="checkbox"> Use Browser for uploads, file duplication, and moving files.</li>
        </ul>
    </div>

    <div class="section">
        <h3>Episode Management</h3>
        <ul>
            <li><input type="checkbox"> Navigate to the specific episode folder (e.g., “animation”/“episode”).</li>
            <li><input type="checkbox"> Right-click on the episode folder > Select Available offline.</li>
            <li><input type="checkbox"> Wait for sync completion in Google Drive app.</li>
        </ul>
    </div>

    <div class="section">
        <h3>Workflow</h3>
        <ul>
            <li><input type="checkbox"> Open Adobe template app after syncing.</li>
            <li><input type="checkbox"> Import the synced media from Google Drive.</li>
            <li><input type="checkbox"> Avoid linking media between projects or episodes.</li>
        </ul>
    </div>

    <div class="section">
        <h3>Exporting & Uploading</h3>
        <ul>
            <li><input type="checkbox"> Export locally, QC offline, and upload H.264 for review.</li>
            <li><input type="checkbox"> Upload QC’d files to Google Drive or Frame.io for team review.</li>
        </ul>
    </div>

    <div class="section">
        <h3>Final Delivery</h3>
        <ul>
            <li><input type="checkbox"> QC and export H.264 and WAV to “Audio Projects > Relevant Episode > Media to Mix.”</li>
            <li><input type="checkbox"> Render and export a ProRes422 file locally, then upload it to Delivery/playout/2.ProRes for Playout.</li>
            <li><input type="checkbox"> Upload checked files to Google Drive or Frame.io for team review.</li>
        </ul>
    </div>

    <div class="section">
        <h3>Backing Up to the Vault</h3>
        <ul>
            <li><input type="checkbox"> Clear unused media to maintain project efficiency.</li>
            <li><input type="checkbox"> Ensure all necessary media in the After Effects project is linked, then select the ‘Main Composition’.</li>
            <li><input type="checkbox"> Go to ‘File’ > ‘Dependencies’ > ‘Collect Files’ and set ‘Collect Source Files’ to ‘For All Comps’.</li>
            <li><input type="checkbox"> Save project to local location (e.g., Desktop) and add ‘_Vault’ to the folder name.</li>
            <li><input type="checkbox"> Upload the consolidated episode folder to the vault on Google Drive.</li>
            <li><input type="checkbox"> Move previous versions to ‘Archive - Do Not Use’ and upload the latest consolidated folder to the top level of the vault.</li>
            <li><input type="checkbox"> Email post@makematic.com, CC’ing your producer upon completion.</li>
        </ul>
    </div>

    <button class="reset-button" onclick="resetChecklist()">Reset Checklist</button>
</div>

<script>
    // Function to reset all checkboxes
    function resetChecklist() {
        const checkboxes = document.querySelectorAll('input[type="checkbox"]');
        checkboxes.forEach(checkbox => checkbox.checked = false);
    }
</script>

</body>
</html>
