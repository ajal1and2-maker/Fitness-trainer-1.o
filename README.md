<!DOCTYPE html>
<html lang="ml">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fitness Tracker</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f9;
            margin: 0;
            padding: 20px;
            display: flex;
            justify-content: center;
        }
        .tracker-card {
            background: #ffffff;
            width: 100%;
            max-width: 600px;
            border: 2px solid #333;
            border-radius: 12px;
            padding: 20px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }
        .header {
            text-align: center;
            border-bottom: 2px solid #333;
            padding-bottom: 10px;
            margin-bottom: 15px;
        }
        .header h1 {
            margin: 0;
            font-size: 24px;
            letter-spacing: 1px;
        }
        .date-section {
            display: flex;
            justify-content: space-between;
            margin-bottom: 15px;
        }
        .date-section input {
            border: none;
            border-bottom: 1px solid #333;
            outline: none;
            padding: 2px 5px;
            width: 30%;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-bottom: 20px;
        }
        th, td {
            border: 1px solid #ccc;
            padding: 6px;
            text-align: center;
            font-size: 13px;
        }
        th {
            background-color: #f0f0f0;
        }
        td input {
            width: 90%;
            border: none;
            outline: none;
            text-align: center;
        }
        .section-title {
            font-weight: bold;
            text-align: center;
            margin: 15px 0 10px 0;
            text-transform: uppercase;
            font-size: 14px;
            letter-spacing: 0.5px;
        }
        .grid-3 {
            display: grid;
            grid-template-columns: 1fr 1fr 1fr;
            gap: 10px;
            margin-bottom: 15px;
        }
        .grid-2 {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 10px;
            margin-bottom: 15px;
        }
        .box {
            border: 1px solid #ccc;
            border-radius: 6px;
            padding: 8px;
            background: #fafafa;
        }
        .box label {
            font-weight: bold;
            font-size: 12px;
            display: block;
            margin-bottom: 5px;
        }
        textarea {
            width: 95%;
            height: 60px;
            border: none;
            background: transparent;
            resize: none;
            outline: none;
        }
        .btn-submit {
            width: 100%;
            padding: 10px;
            background-color: #28a745;
            color: white;
            border: none;
            border-radius: 6px;
            font-size: 16px;
            cursor: pointer;
        }
        .btn-submit:hover {
            background-color: #218838;
        }
    </style>
</head>
<body>

<div class="tracker-card">
    <div class="header">
        <h1>FITNESS TRACKER 🏃</h1>
        <small>MOVE YOUR BODY, STAY MOTIVATED</small>
    </div>

    <div class="date-section">
        <input type="text" placeholder="Day: Monday">
        <input type="date">
        <input type="text" placeholder="Year: 2026">
    </div>

    <table>
        <thead>
            <tr>
                <th>Workout Routine 🏢</th>
                <th>Sets 🏋️</th>
                <th>Reps 🔄</th>
                <th>Weight ⚖️</th>
                <th>Time ⏱️</th>
            </tr>
        </thead>
        <tbody>
            <!-- 5 Rows for workouts -->
            <tr><td><input type="text"></td><td><input type="text"></td><td><input type="text"></td><td><input type="text"></td><td><input type="text"></td></tr>
            <tr><td><input type="text"></td><td><input type="text"></td><td><input type="text"></td><td><input type="text"></td><td><input type="text"></td></tr>
            <tr><td><input type="text"></td><td><input type="text"></td><td><input type="text"></td><td><input type="text"></td><td><input type="text"></td></tr>
            <tr><td><input type="text"></td><td><input type="text"></td><td><input type="text"></td><td><input type="text"></td><td><input type="text"></td></tr>
            <tr><td><input type="text"></td><td><input type="text"></td><td><input type="text"></td><td><input type="text"></td><td><input type="text"></td></tr>
        </tbody>
    </table>

    <div class="section-title">Daily Nutrition Tracker</div>
    <div class="grid-3">
        <div class="box">
            <label>Morning ☀️</label>
            <textarea placeholder="Breakfast & snacks..."></textarea>
        </div>
        <div class="box">
            <label>Afternoon 🌤️</label>
            <textarea placeholder="Lunch..."></textarea>
        </div>
        <div class="box">
            <label>Evening 🌙</label>
            <textarea placeholder="Dinner & snacks..."></textarea>
        </div>
    </div>

    <div class="grid-2">
        <div class="box">
            <label>Water Intake 💧</label>
            <input type="text" style="width:100%; border:none;" placeholder="e.g. 3 Liters / 8 Glasses">
        </div>
        <div class="box">
            <label>Sleep Hours 🌙</label>
            <input type="text" style="width:100%; border:none;" placeholder="e.g. 7 Hours">
        </div>
    </div>

    <div class="grid-2">
        <div class="box">
            <label>Fitness Goals 🏕️</label>
            <textarea placeholder="Today's goal..."></textarea>
        </div>
        <div class="box">
            <label>Reminder 📌</label>
            <textarea placeholder="Notes / Reminders..."></textarea>
        </div>
    </div>

    <button class="btn-submit" onclick="alert('തത്സമയം ഡാറ്റ രേഖപ്പെടുത്തി!')">Save Today's Entry</button>
</div>

</body>
</html>
