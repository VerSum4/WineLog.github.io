<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>WineLog - Weinbehandlungen</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
        }

        header {
            background-color: #8a2b06;
            color: white;
            padding: 10px 20px;
            text-align: center;
        }

        .container {
            margin: 20px auto;
            max-width: 800px;
            padding: 20px;
            background-color: white;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
        }

        table th, table td {
            padding: 10px;
            text-align: left;
            border-bottom: 1px solid #ddd;
        }

        button {
            padding: 10px 15px;
            background-color: #8a2b06;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        button:hover {
            background-color: #6b2204;
        }

        input, select, textarea {
            width: calc(100% - 22px);
            padding: 10px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <header>
        <h1>WineLog - Dokumentation von Weinbehandlungen</h1>
    </header>

    <div class="container">
        <h2>Neue Behandlung hinzufügen</h2>
        <form id="entryForm">
            <input type="date" id="date" required placeholder="Datum">
            <select id="treatmentType" required>
                <option value="">Behandlungstyp auswählen</option>
                <option value="Schwefelung">Schwefelung</option>
                <option value="Filtration">Filtration</option>
                <option value="Lagerung">Lagerung</option>
            </select>

            <textarea id="tanknummer" rows="1" placeholder="Tanknummer (optional)"></textarea>
            <textarea id="notes" rows="4" placeholder="Notizen (optional)"></textarea>
            <button type="submit">Hinzufügen</button>
        </form>

        <h2>Behandlungen</h2>
        <table id="entriesTable">
            <thead>
                <tr>
                    <th>Datum</th>
                    <th>Behandlungstyp</th>
                    <th>Tanknummer</th>
                    <th>Notizen</th>
                    <th>Aktionen</th>
                </tr>
            </thead>
            <tbody>
                <!-- Dynamische Einträge -->
            </tbody>
        </table>
    </div>

    <script>
        const form = document.getElementById('entryForm');
        const tableBody = document.querySelector('#entriesTable tbody');
        let entries = JSON.parse(localStorage.getItem('entries')) || [];

        function renderEntries() {
            tableBody.innerHTML = '';
            entries.forEach((entry, index) => {
                const row = document.createElement('tr');
                row.innerHTML = `
                    <td>${entry.date}</td>
                    <td>${entry.treatmentType}</td>
                    <td>${entry.tanknummer}</td>
                    <td>${entry.notes}</td>
                    <td>
                        <button onclick="deleteEntry(${index})">Löschen</button>
                    </td>
                `;
                tableBody.appendChild(row);
            });
        }

        function deleteEntry(index) {
            entries.splice(index, 1);
            localStorage.setItem('entries', JSON.stringify(entries));
            renderEntries();
        }

        form.addEventListener('submit', (e) => {
            e.preventDefault();

            const newEntry = {
                date: document.getElementById('date').value,
                treatmentType: document.getElementById('treatmentType').value,
                notes: document.getElementById('notes').value || 'Keine Notizen',
                tanknummer: document.getElementById('tanknummer').value || 'Keine Tanknummer'
            };

            entries.push(newEntry);
            localStorage.setItem('entries', JSON.stringify(entries));
            form.reset();
            renderEntries();
        });

        // Initiales Rendern
        renderEntries();
    </script>
</body>
</html>

