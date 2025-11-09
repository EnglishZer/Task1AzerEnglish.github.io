
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>English for Azerbaijani Kids</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #25D366 0%, #128C7E 100%);
            min-height: 100vh;
            padding: 10px;
            color: #333;
        }
        
        .container {
            max-width: 100%;
            background-color: white;
            border-radius: 15px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            overflow: hidden;
        }
        
        header {
            text-align: center;
            padding: 15px;
            background: #128C7E;
            color: white;
        }
        
        h1 {
            font-size: 1.5rem;
            margin-bottom: 5px;
        }
        
        .subtitle {
            font-size: 0.9rem;
            opacity: 0.9;
        }
        
        .nav-tabs {
            display: flex;
            overflow-x: auto;
            padding: 10px;
            background: #f0f0f0;
            gap: 5px;
            -webkit-overflow-scrolling: touch;
        }
        
        .tab {
            padding: 8px 12px;
            background-color: white;
            border: none;
            border-radius: 20px;
            cursor: pointer;
            font-size: 0.8rem;
            font-weight: bold;
            white-space: nowrap;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
        
        .tab.active {
            background-color: #25D366;
            color: white;
        }
        
        .content {
            padding: 10px;
            min-height: 300px;
        }
        
        .category {
            display: none;
        }
        
        .category.active {
            display: block;
        }
        
        .cards-container {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 10px;
        }
        
        .card {
            background-color: white;
            border-radius: 10px;
            padding: 10px;
            box-shadow: 0 2px 6px rgba(0, 0, 0, 0.1);
            text-align: center;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        
        .card img {
            width: 100%;
            height: 80px;
            object-fit: cover;
            border-radius: 8px;
            margin-bottom: 8px;
        }
        
        .word {
            font-size: 1rem;
            color: #128C7E;
            margin-bottom: 3px;
            font-weight: bold;
        }
        
        .translation {
            font-size: 0.9rem;
            color: #25D366;
            margin-bottom: 8px;
        }
        
        .audio-btn {
            background-color: #25D366;
            color: white;
            border: none;
            border-radius: 50%;
            width: 36px;
            height: 36px;
            font-size: 0.9rem;
            cursor: pointer;
        }
        
        .game-container {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 8px;
        }
        
        .game-card {
            background-color: white;
            border-radius: 8px;
            padding: 12px 8px;
            text-align: center;
            cursor: pointer;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            min-height: 60px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 0.9rem;
        }
        
        .game-card.selected {
            background-color: #25D366;
            color: white;
        }
        
        .game-card.matched {
            background-color: #128C7E;
            color: white;
        }
        
        .progress-container {
            margin-top: 15px;
            background-color: #f0f0f0;
            border-radius: 8px;
            overflow: hidden;
        }
        
        .progress-bar {
            height: 15px;
            background-color: #25D366;
            width: 0%;
            transition: width 0.3s;
        }
        
        .progress-text {
            text-align: center;
            padding: 8px;
            font-size: 0.9rem;
        }
        
        .instructions {
            text-align: center;
            padding: 10px;
            font-size: 0.8rem;
            color: #666;
            background: #f9f9f9;
            border-radius: 8px;
            margin: 10px 0;
        }
        
        /* WhatsApp-like styles */
        .whatsapp-header {
            display: flex;
            align-items: center;
            padding: 10px 15px;
            background: #128C7E;
            color: white;
        }
        
        .whatsapp-back {
            margin-right: 15px;
            font-size: 1.2rem;
        }
        
        .whatsapp-title {
            flex-grow: 1;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="whatsapp-header">
            <div class="whatsapp-back">←</div>
            <div class="whatsapp-title">
                <h1>English for Azerbaijani Kids</h1>
            </div>
        </div>
        
        <div class="nav-tabs">
            <button class="tab active" data-category="animals">Animals</button>
            <button class="tab" data-category="food">Food</button>
            <button class="tab" data-category="colors">Colors</button>
            <button class="tab" data-category="numbers">Numbers</button>
            <button class="tab" data-category="family">Family</button>
            <button class="tab" data-category="game">Game</button>
        </div>
        
        <div class="content">
            <!-- Animals Category -->
            <div class="category active" id="animals">
                <div class="instructions">Tap the 🔊 button to hear pronunciation</div>
                <div class="cards-container">
                    <div class="card">
                        <img src="https://images.unsplash.com/photo-1543852786-1cf6624b9987?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MTB8fGNhdHxlbnwwfHwwfHx8MA%3D%3D&auto=format&fit=crop&w=200&q=60" alt="Cat">
                        <div class="word">Cat</div>
                        <div class="translation">Pişik</div>
                        <button class="audio-btn" data-word="cat">🔊</button>
                    </div>
                    <div class="card">
                        <img src="https://images.unsplash.com/photo-1552053831-71594a27632d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8M3x8ZG9nfGVufDB8fDB8fHww&auto=format&fit=crop&w=200&q=60" alt="Dog">
                        <div class="word">Dog</div>
                        <div class="translation">İt</div>
                        <button class="audio-btn" data-word="dog">🔊</button>
                    </div>
                    <div class="card">
                        <img src="https://images.unsplash.com/photo-1546445317-29f4545e9d53?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MTJ8fGNvd3xlbnwwfHwwfHx8MA%3D%3D&auto=format&fit=crop&w=200&q=60" alt="Cow">
                        <div class="word">Cow</div>
                        <div class="translation">İnək</div>
                        <button class="audio-btn" data-word="cow">🔊</button>
                    </div>
                    <div class="card">
                        <img src="https://images.unsplash.com/photo-1555169062-013468b47731?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8NHx8YmlyZHxlbnwwfHwwfHx8MA%3D%3D&auto=format&fit=crop&w=200&q=60" alt="Bird">
                        <div class="word">Bird</div>
                        <div class="translation">Quş</div>
                        <button class="audio-btn" data-word="bird">🔊</button>
                    </div>
                </div>
            </div>
            
            <!-- Food Category -->
            <div class="category" id="food">
                <div class="instructions">Tap the 🔊 button to hear pronunciation</div>
                <div class="cards-container">
                    <div class="card">
                        <img src="https://images.unsplash.com/photo-1568702846914-96b305d2aaeb?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MTJ8fGFwcGxlfGVufDB8fDB8fHww&auto=format&fit=crop&w=200&q=60" alt="Apple">
                        <div class="word">Apple</div>
                        <div class="translation">Alma</div>
                        <button class="audio-btn" data-word="apple">🔊</button>
                    </div>
                    <div class="card">
                        <img src="https://images.unsplash.com/photo-1509440159596-0249088772ff?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MTJ8fGJyZWFkfGVufDB8fDB8fHww&auto=format&fit=crop&w=200&q=60" alt="Bread">
                        <div class="word">Bread</div>
                        <div class="translation">Çörək</div>
                        <button class="audio-btn" data-word="bread">🔊</button>
                    </div>
                    <div class="card">
                        <img src="https://images.unsplash.com/photo-1563636619-e9143da7973b?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MTJ8fG1pbGt8ZW58MHx8MHx8fDA%3D&auto=format&fit=crop&w=200&q=60" alt="Milk">
                        <div class="word">Milk</div>
                        <div class="translation">Süd</div>
                        <button class="audio-btn" data-word="milk">🔊</button>
                    </div>
                    <div class="card">
                        <img src="https://images.unsplash.com/photo-1551189753-9dfd7cd19056?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MTJ8fHdhdGVyfGVufDB8fDB8fHww&auto=format&fit=crop&w=200&q=60" alt="Water">
                        <div class="word">Water</div>
                        <div class="translation">Su</div>
                        <button class="audio-btn" data-word="water">🔊</button>
                    </div>
                </div>
            </div>
            
            <!-- Colors Category -->
            <div class="category" id="colors">
                <div class="instructions">Tap the 🔊 button to hear pronunciation</div>
                <div class="cards-container">
                    <div class="card">
                        <div style="width: 100%; height: 80px; background-color: #FF6B6B; border-radius: 8px; margin-bottom: 8px;"></div>
                        <div class="word">Red</div>
                        <div class="translation">Qırmızı</div>
                        <button class="audio-btn" data-word="red">🔊</button>
                    </div>
                    <div class="card">
                        <div style="width: 100%; height: 80px; background-color: #4ECDC4; border-radius: 8px; margin-bottom: 8px;"></div>
                        <div class="word">Blue</div>
                        <div class="translation">Göy</div>
                        <button class="audio-btn" data-word="blue">🔊</button>
                    </div>
                    <div class="card">
                        <div style="width: 100%; height: 80px; background-color: #6BCF7F; border-radius: 8px; margin-bottom: 8px;"></div>
                        <div class="word">Green</div>
                        <div class="translation">Yaşıl</div>
                        <button class="audio-btn" data-word="green">🔊</button>
                    </div>
                    <div class="card">
                        <div style="width: 100%; height: 80px; background-color: #FFD93D; border-radius: 8px; margin-bottom: 8px;"></div>
                        <div class="word">Yellow</div>
                        <div class="translation">Sarı</div>
                        <button class="audio-btn" data-word="yellow">🔊</button>
                    </div>
                </div>
            </div>
            
            <!-- Numbers Category -->
            <div class="category" id="numbers">
                <div class="instructions">Tap the 🔊 button to hear pronunciation</div>
                <div class="cards-container">
                    <div class="card">
                        <div style="width: 100%; height: 80px; display: flex; align-items: center; justify-content: center; font-size: 2.5rem; color: #FF6B6B; margin-bottom: 8px;">1</div>
                        <div class="word">One</div>
                        <div class="translation">Bir</div>
                        <button class="audio-btn" data-word="one">🔊</button>
                    </div>
                    <div class="card">
                        <div style="width: 100%; height: 80px; display: flex; align-items: center; justify-content: center; font-size: 2.5rem; color: #4ECDC4; margin-bottom: 8px;">2</div>
                        <div class="word">Two</div>
                        <div class="translation">İki</div>
                        <button class="audio-btn" data-word="two">🔊</button>
                    </div>
                    <div class="card">
                        <div style="width: 100%; height: 80px; display: flex; align-items: center; justify-content: center; font-size: 2.5rem; color: #6BCF7F; margin-bottom: 8px;">3</div>
                        <div class="word">Three</div>
                        <div class="translation">Üç</div>
                        <button class="audio-btn" data-word="three">🔊</button>
                    </div>
                    <div class="card">
                        <div style="width: 100%; height: 80px; display: flex; align-items: center; justify-content: center; font-size: 2.5rem; color: #FFD93D; margin-bottom: 8px;">4</div>
                        <div class="word">Four</div>
                        <div class="translation">Dörd</div>
                        <button class="audio-btn" data-word="four">🔊</button>
                    </div>
                </div>
            </div>
            
            <!-- Family Category -->
            <div class="category" id="family">
                <div class="instructions">Tap the 🔊 button to hear pronunciation</div>
                <div class="cards-container">
                    <div class="card">
                        <img src="https://images.unsplash.com/photo-1519456264917-42d0aa2e0625?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MTJ8fG1vdGhlcnxlbnwwfHwwfHx8MA%3D%3D&auto=format&fit=crop&w=200&q=60" alt="Mother">
                        <div class="word">Mother</div>
                        <div class="translation">Ana</div>
                        <button class="audio-btn" data-word="mother">🔊</button>
                    </div>
                    <div class="card">
                        <img src="https://images.unsplash.com/photo-1567532939604-b6b5b0db2604?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MTJ8fGZhdGhlcnxlbnwwfHwwfHx8MA%3D%3D&auto=format&fit=crop&w=200&q=60" alt="Father">
                        <div class="word">Father</div>
                        <div class="translation">Ata</div>
                        <button class="audio-btn" data-word="father">🔊</button>
                    </div>
                    <div class="card">
                        <img src="https://images.unsplash.com/photo-1519456264917-42d0aa2e0625?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MTJ8fHNpc3RlcnxlbnwwfHwwfHx8MA%3D%3D&auto=format&fit=crop&w=200&q=60" alt="Sister">
                        <div class="word">Sister</div>
                        <div class="translation">Bacı</div>
                        <button class="audio-btn" data-word="sister">🔊</button>
                    </div>
                    <div class="card">
                        <img src="https://images.unsplash.com/photo-1567532939604-b6b5b0db2604?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MTJ8fGJyb3RoZXJ8ZW58MHx8MHx8fDA%3D&auto=format&fit=crop&w=200&q=60" alt="Brother">
                        <div class="word">Brother</div>
                        <div class="translation">Qardaş</div>
                        <button class="audio-btn" data-word="brother">🔊</button>
                    </div>
                </div>
            </div>
            
            <!-- Matching Game -->
            <div class="category" id="game">
                <div class="instructions">Match English words with Azerbaijani translations</div>
                <div class="game-container" id="game-container">
                    <!-- Game cards will be generated by JavaScript -->
                </div>
                <div class="progress-container">
                    <div class="progress-bar" id="progress-bar"></div>
                    <div class="progress-text" id="progress-text">Progress: 0%</div>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Tab navigation
        document.querySelectorAll('.tab').forEach(tab => {
            tab.addEventListener('click', () => {
                // Remove active class from all tabs and categories
                document.querySelectorAll('.tab').forEach(t => t.classList.remove('active'));
                document.querySelectorAll('.category').forEach(c => c.classList.remove('active'));
                
                // Add active class to clicked tab and corresponding category
                tab.classList.add('active');
                const categoryId = tab.getAttribute('data-category');
                document.getElementById(categoryId).classList.add('active');
                
                // If game tab is clicked, initialize the game
                if (categoryId === 'game') {
                    initializeGame();
                }
            });
        });
        
        // Audio pronunciation
        document.querySelectorAll('.audio-btn').forEach(button => {
            button.addEventListener('click', () => {
                const word = button.getAttribute('data-word');
                speakWord(word);
            });
        });
        
        // Text-to-speech function
        function speakWord(word) {
            if ('speechSynthesis' in window) {
                const utterance = new SpeechSynthesisUtterance(word);
                utterance.lang = 'en-US';
                utterance.rate = 0.8; // Slower for children
                speechSynthesis.speak(utterance);
            } else {
                alert('Audio not supported in this browser');
            }
        }
        
        // Matching Game
        let selectedCards = [];
        let matchedPairs = 0;
        let totalPairs = 0;
        
        function initializeGame() {
            const gameContainer = document.getElementById('game-container');
            gameContainer.innerHTML = '';
            selectedCards = [];
            matchedPairs = 0;
            
            // Word pairs for the matching game
            const wordPairs = [
                { english: 'Cat', azerbaijani: 'Pişik' },
                { english: 'Dog', azerbaijani: 'İt' },
                { english: 'Apple', azerbaijani: 'Alma' },
                { english: 'Red', azerbaijani: 'Qırmızı' },
                { english: 'One', azerbaijani: 'Bir' },
                { english: 'Mother', azerbaijani: 'Ana' }
            ];
            
            totalPairs = wordPairs.length;
            
            // Create an array with both English and Azerbaijani words
            let gameWords = [];
            wordPairs.forEach(pair => {
                gameWords.push({ text: pair.english, type: 'english', pairId: pair.english });
                gameWords.push({ text: pair.azerbaijani, type: 'azerbaijani', pairId: pair.english });
            });
            
            // Shuffle the array
            gameWords = shuffleArray(gameWords);
            
            // Create game cards
            gameWords.forEach(word => {
                const card = document.createElement('div');
                card.className = 'game-card';
                card.textContent = word.text;
                card.setAttribute('data-type', word.type);
                card.setAttribute('data-pair-id', word.pairId);
                card.addEventListener('click', () => selectCard(card));
                gameContainer.appendChild(card);
            });
            
            updateProgress();
        }
        
        function shuffleArray(array) {
            for (let i = array.length - 1; i > 0; i--) {
                const j = Math.floor(Math.random() * (i + 1));
                [array[i], array[j]] = [array[j], array[i]];
            }
            return array;
        }
        
        function selectCard(card) {
            // If card is already selected or matched, do nothing
            if (card.classList.contains('selected') || card.classList.contains('matched')) {
                return;
            }
            
            // If two cards are already selected, do nothing
            if (selectedCards.length >= 2) {
                return;
            }
            
            // Select the card
            card.classList.add('selected');
            selectedCards.push(card);
            
            // If two cards are selected, check for a match
            if (selectedCards.length === 2) {
                const card1 = selectedCards[0];
                const card2 = selectedCards[1];
                
                // Check if the cards are a match
                if (card1.getAttribute('data-pair-id') === card2.getAttribute('data-pair-id') && 
                    card1.getAttribute('data-type') !== card2.getAttribute('data-type')) {
                    // Match found
                    setTimeout(() => {
                        card1.classList.remove('selected');
                        card2.classList.remove('selected');
                        card1.classList.add('matched');
                        card2.classList.add('matched');
                        selectedCards = [];
                        matchedPairs++;
                        updateProgress();
                        
                        // Check if all pairs are matched
                        if (matchedPairs === totalPairs) {
                            setTimeout(() => {
                                alert('Təbriklər! Bütün cütləri tapdınız!');
                            }, 500);
                        }
                    }, 500);
                } else {
                    // Not a match
                    setTimeout(() => {
                        card1.classList.remove('selected');
                        card2.classList.remove('selected');
                        selectedCards = [];
                    }, 1000);
                }
            }
        }
        
        function updateProgress() {
            const progress = (matchedPairs / totalPairs) * 100;
            const progressBar = document.getElementById('progress-bar');
            const progressText = document.getElementById('progress-text');
            
            progressBar.style.width = `${progress}%`;
            progressText.textContent = `Progress: ${Math.round(progress)}%`;
        }
        
        // Initialize the first category
        initializeGame();
    </script>
</body>
</html>
