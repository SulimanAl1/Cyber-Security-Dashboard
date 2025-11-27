   document.addEventListener('DOMContentLoaded', function() {
       fetch('data/attacks_log.json')
           .then(response => response.json())
           .then(data => {
               const attacksDiv = document.getElementById('attacks');
               const summaryDiv = document.getElementById('summary');
               const searchInput = document.getElementById('search');

               // Generate daily summary
               const today = new Date().toISOString().split('T')[0];
               const todayAttacks = data.attacks.filter(a => a.date === today);
               summaryDiv.innerHTML = `<h2>Daily Summary (${today})</h2><p>${todayAttacks.length} attacks reported.</p>`;

               // Display all attacks
               function displayAttacks(attacks) {
                   attacksDiv.innerHTML = '';
                   attacks.forEach(attack => {
                       const div = document.createElement('div');
                       div.className = 'attack';
                       div.innerHTML = `
                           <h3>${attack.impact_target}</h3>
                           <p><strong>Method:</strong> ${attack.attack_method}</p>
                           <p><strong>Attacker:</strong> ${attack.attacker_group}</p>
                           <p><strong>Cost:</strong> ${attack.financial_cost}</p>
                           <p><strong>Remediation:</strong> ${attack.remediation}</p>
                           <p><strong>Date:</strong> ${attack.date}</p>
                       `;
                       attacksDiv.appendChild(div);
                   });
               }
               displayAttacks(data.attacks);

               // Search functionality
               searchInput.addEventListener('input', function() {
                   const query = this.value.toLowerCase();
                   const filtered = data.attacks.filter(a =>
                       a.impact_target.toLowerCase().includes(query) ||
                       a.attack_method.toLowerCase().includes(query)
                   );
                   displayAttacks(filtered);
               });
           })
           .catch(error => console.error('Error loading data:', error));
   });
   
