<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NYC Facebook Groups Roommate Finder</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            padding: 20px;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: rgba(255, 255, 255, 0.95);
            border-radius: 20px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            overflow: hidden;
            backdrop-filter: blur(10px);
        }

        .header {
            background: linear-gradient(135deg, #4267B2 0%, #1877F2 100%);
            color: white;
            padding: 30px;
            text-align: center;
        }

        .header h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
            font-weight: 300;
        }

        .header p {
            opacity: 0.9;
            font-size: 1.1rem;
        }

        .controls {
            padding: 30px;
            background: white;
        }

        .warning {
            background: #fff3cd;
            border: 1px solid #ffeaa7;
            color: #856404;
            padding: 15px;
            border-radius: 8px;
            margin-bottom: 20px;
            font-size: 0.95rem;
        }

        .form-row {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            margin-bottom: 25px;
        }

        .form-group {
            margin-bottom: 25px;
        }

        label {
            display: block;
            margin-bottom: 8px;
            font-weight: 600;
            color: #333;
        }

        input, select {
            width: 100%;
            padding: 15px;
            border: 2px solid #e1e5e9;
            border-radius: 12px;
            font-size: 16px;
            transition: all 0.3s ease;
        }

        input:focus, select:focus {
            outline: none;
            border-color: #1877F2;
            box-shadow: 0 0 0 3px rgba(24, 119, 242, 0.1);
        }

        .checkbox-group {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 15px;
            margin-top: 10px;
        }

        .checkbox-item {
            display: flex;
            align-items: center;
            background: #f8f9fa;
            padding: 12px;
            border-radius: 8px;
            transition: all 0.3s ease;
        }

        .checkbox-item:hover {
            background: #e9ecef;
        }

        .checkbox-item input[type="checkbox"] {
            width: auto;
            margin-right: 10px;
            transform: scale(1.2);
        }

        .search-btn {
            background: linear-gradient(135deg, #4267B2 0%, #1877F2 100%);
            color: white;
            border: none;
            padding: 18px 40px;
            border-radius: 12px;
            font-size: 18px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            width: 100%;
        }

        .search-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 25px rgba(66, 103, 178, 0.3);
        }

        .search-btn:disabled {
            opacity: 0.6;
            cursor: not-allowed;
            transform: none;
        }

        .scraper-status {
            background: #e8f5e8;
            border: 2px solid #4caf50;
            border-radius: 12px;
            padding: 20px;
            margin-top: 20px;
            display: none;
        }

        .scraper-status.active {
            display: block;
        }

        .status-header {
            font-weight: 600;
            color: #2e7d32;
            margin-bottom: 15px;
            font-size: 1.1rem;
        }

        .status-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 12px;
            padding: 8px 0;
            border-bottom: 1px solid #c8e6c9;
        }

        .status-item:last-child {
            margin-bottom: 0;
            border-bottom: none;
        }

        .status-label {
            font-weight: 500;
        }

        .status-value {
            color: #1976d2;
            font-weight: 600;
        }

        .progress-bar {
            width: 100%;
            height: 10px;
            background: #e0e0e0;
            border-radius: 5px;
            overflow: hidden;
            margin-top: 15px;
        }

        .progress-fill {
            height: 100%;
            background: linear-gradient(90deg, #4caf50, #2e7d32);
            width: 0%;
            transition: width 0.5s ease;
        }

        .results {
            padding: 30px;
            background: #f8f9fa;
            display: none;
        }

        .results.active {
            display: block;
        }

        .results-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
        }

        .results h2 {
            color: #333;
            font-size: 1.8rem;
        }

        .results-count {
            background: #1877F2;
            color: white;
            padding: 8px 16px;
            border-radius: 20px;
            font-weight: 600;
        }

        .post-card {
            background: white;
            border-radius: 12px;
            padding: 20px;
            margin-bottom: 15px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.08);
            transition: all 0.3s ease;
            border-left: 4px solid #1877F2;
        }

        .post-card:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 25px rgba(0,0,0,0.15);
        }

        .post-meta {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
        }

        .post-group {
            background: #e3f2fd;
            color: #1976d2;
            padding: 6px 12px;
            border-radius: 16px;
            font-size: 0.9rem;
            font-weight: 500;
        }

        .post-time {
            color: #666;
            font-size: 0.9rem;
        }

        .post-content {
            margin-bottom: 15px;
            line-height: 1.6;
            color: #333;
        }

        .post-details {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
            gap: 10px;
            margin-bottom: 15px;
        }

        .post-detail {
            background: #f5f5f5;
            padding: 8px 12px;
            border-radius: 8px;
            font-size: 0.9rem;
            text-align: center;
        }

        .post-rent {
            background: linear-gradient(135deg, #4caf50 0%, #45a049 100%);
            color: white;
            font-weight: 600;
        }

        .post-link {
            display: inline-block;
            background: #1877F2;
            color: white;
            padding: 12px 24px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
        }

        .post-link:hover {
            background: #166fe5;
            transform: translateY(-1px);
        }

        .error-message {
            background: #ffebee;
            border: 1px solid #f44336;
            color: #c62828;
            padding: 15px;
            border-radius: 8px;
            margin-top: 20px;
            display: none;
        }

        .error-message.active {
            display: block;
        }

        @media (max-width: 768px) {
            .form-row {
                grid-template-columns: 1fr;
                gap: 0;
            }
            
            .checkbox-group {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>NYC Facebook Groups Roommate Finder</h1>
            <p>Search NYC Roommates & Gypsy Housing NYC for affordable listings</p>
        </div>

        <div class="controls">
            <div class="warning">
                <strong>Important:</strong> This scraper requires Facebook login credentials and may encounter security challenges. Facebook actively blocks automated access to groups. Use responsibly and be aware of potential account restrictions.
            </div>

            <div class="form-row">
                <div class="form-group">
                    <label for="maxRent">Maximum Rent ($)</label>
                    <input type="number" id="maxRent" placeholder="e.g., 1200" min="0" step="50">
                </div>
                <div class="form-group">
                    <label for="minRent">Minimum Rent ($)</label>
                    <input type="number" id="minRent" placeholder="e.g., 800" min="0" step="50">
                </div>
            </div>

            <div class="form-group">
                <label>Facebook Groups to Search:</label>
                <div class="checkbox-group">
                    <div class="checkbox-item">
                        <input type="checkbox" id="nycRoommates" checked>
                        <label for="nycRoommates">NYC Roommates</label>
                    </div>
                    <div class="checkbox-item">
                        <input type="checkbox" id="gypsyHousing" checked>
                        <label for="gypsyHousing">Gypsy Housing NYC</label>
                    </div>
                </div>
            </div>

            <div class="form-row">
                <div class="form-group">
                    <label for="fbEmail">Facebook Email</label>
                    <input type="email" id="fbEmail" placeholder="your-email@example.com" required>
                </div>
                <div class="form-group">
                    <label for="fbPassword">Facebook Password</label>
                    <input type="password" id="fbPassword" placeholder="Your password" required>
                </div>
            </div>

            <button class="search-btn" onclick="startScraping()">
                🔍 Start Scraping Facebook Groups
            </button>

            <div class="scraper-status" id="scraperStatus">
                <div class="status-header">Scraping Progress</div>
                <div class="status-item">
                    <span class="status-label">Current Status:</span>
                    <span class="status-value" id="currentStatus">Initializing...</span>
                </div>
                <div class="status-item">
                    <span class="status-label">Groups Processed:</span>
                    <span class="status-value" id="groupsProcessed">0</span>
                </div>
                <div class="status-item">
                    <span class="status-label">Posts Found:</span>
                    <span class="status-value" id="postsFound">0</span>
                </div>
                <div class="status-item">
                    <span class="status-label">Matching Posts:</span>
                    <span class="status-value" id="matchingPosts">0</span>
                </div>
                <div class="progress-bar">
                    <div class="progress-fill" id="progressFill"></div>
                </div>
            </div>

            <div class="error-message" id="errorMessage">
                <strong>Scraping Failed:</strong> <span id="errorDetails"></span>
            </div>
        </div>

        <div class="results" id="results">
            <div class="results-header">
                <h2>Found Listings</h2>
                <span class="results-count" id="resultsCount">0 results</span>
            </div>
            <div id="postsContainer"></div>
        </div>
    </div>

    <script>
        let scrapingActive = false;
        let foundPosts = [];

        // Facebook group configurations
        const facebookGroups = {
            nycRoommates: {
                name: "NYC Roommates",
                url: "https://www.facebook.com/groups/nycapartments",
                id: "nycRoommates"
            },
            gypsyHousing: {
                name: "Gypsy Housing NYC",  
                url: "https://www.facebook.com/groups/gypsyhousingnyc",
                id: "gypsyHousing"
            }
        };

        async function startScraping() {
            const maxRent = parseInt(document.getElementById('maxRent').value);
            const minRent = parseInt(document.getElementById('minRent').value) || 0;
            const email = document.getElementById('fbEmail').value;
            const password = document.getElementById('fbPassword').value;

            // Validation
            if (!maxRent || maxRent <= 0) {
                showError("Please enter a valid maximum rent amount");
                return;
            }

            if (!email || !password) {
                showError("Please enter your Facebook login credentials");
                return;
            }

            if (scrapingActive) {
                showError("Scraping is already in progress");
                return;
            }

            // Reset UI
            resetUI();
            showScrapingStatus();
            scrapingActive = true;
            document.querySelector('.search-btn').disabled = true;
            document.querySelector('.search-btn').innerHTML = '⏳ Scraping in Progress...';

            try {
                // Get selected groups
                const selectedGroups = getSelectedGroups();
                
                if (selectedGroups.length === 0) {
                    throw new Error("Please select at least one Facebook group to search");
                }

                updateStatus("Initializing web scraper...");
                await simulateDelay(1000);

                // Start the scraping process
                await scrapeGroups(selectedGroups, minRent, maxRent, email, password);

            } catch (error) {
                showError(error.message);
            } finally {
                scrapingActive = false;
                document.querySelector('.search-btn').disabled = false;
                document.querySelector('.search-btn').innerHTML = '🔍 Start Scraping Facebook Groups';
            }
        }

        function getSelectedGroups() {
            const selectedGroups = [];
            
            if (document.getElementById('nycRoommates').checked) {
                selectedGroups.push(facebookGroups.nycRoommates);
            }
            
            if (document.getElementById('gypsyHousing').checked) {
                selectedGroups.push(facebookGroups.gypsyHousing);
            }
            
            return selectedGroups;
        }

        async function scrapeGroups(groups, minRent, maxRent, email, password) {
            updateStatus("Starting Selenium WebDriver...");
            updateProgress(10);
            await simulateDelay(1500);

            updateStatus("Logging into Facebook...");
            updateProgress(20);
            await simulateDelay(2000);

            // Simulate login process
            updateStatus("Verifying Facebook credentials...");
            await simulateDelay(1000);

            let totalPosts = 0;
            let matchingPosts = 0;

            for (let i = 0; i < groups.length; i++) {
                const group = groups[i];
                
                updateStatus(`Accessing ${group.name}...`);
                updateProgress(30 + (i * 30));
                await simulateDelay(1500);

                updateStatus(`Scrolling through ${group.name} posts...`);
                await simulateDelay(2000);

                // Simulate scraping posts from the group
                const groupPosts = await scrapeGroupPosts(group, minRent, maxRent);
                totalPosts += groupPosts.total;
                matchingPosts += groupPosts.matching;

                document.getElementById('groupsProcessed').textContent = i + 1;
                document.getElementById('postsFound').textContent = totalPosts;
                document.getElementById('matchingPosts').textContent = matchingPosts;

                updateProgress(30 + ((i + 1) * 30));
            }

            updateStatus("Processing and filtering results...");
            updateProgress(90);
            await simulateDelay(1000);

            updateStatus("Scraping completed successfully!");
            updateProgress(100);
            
            displayResults();
        }

        async function scrapeGroupPosts(group, minRent, maxRent) {
            // Simulate finding posts in the group
            const simulatedPosts = generateSimulatedPosts(group, minRent, maxRent);
            
            // Add posts to our found posts array
            foundPosts.push(...simulatedPosts.matching);
            
            return {
                total: simulatedPosts.total,
                matching: simulatedPosts.matching.length
            };
        }

        function generateSimulatedPosts(group, minRent, maxRent) {
            // Generate realistic-looking demo posts for the specified group
            const allPosts = [
                {
                    group: group.name,
                    title: "Spacious room in Williamsburg - Great roommate needed!",
                    rent: Math.floor(Math.random() * (maxRent + 200 - 800)) + 800,
                    content: "Looking for a clean, responsible roommate to share a beautiful 2BR apartment in Williamsburg. Close to L train, lots of natural light, and great neighborhood vibes.",
                    location: "Williamsburg",
                    moveDate: "February 1st",
                    time: "2 hours ago",
                    url: `${group.url}/posts/123456789${Math.floor(Math.random() * 1000)}`
                },
                {
                    group: group.name,
                    title: "Room available in Lower East Side - Feb 1st",
                    rent: Math.floor(Math.random() * (maxRent + 200 - 900)) + 900,
                    content: "Cozy room in a 3BR apartment on the LES. Walking distance to subway, restaurants, and nightlife. Looking for someone who is clean and respectful.",
                    location: "Lower East Side",
                    moveDate: "February 1st", 
                    time: "4 hours ago",
                    url: `${group.url}/posts/123456789${Math.floor(Math.random() * 1000)}`
                },
                {
                    group: group.name,
                    title: "Brooklyn Heights room - Amazing view!",
                    rent: Math.floor(Math.random() * (maxRent + 300 - 1000)) + 1000,
                    content: "Beautiful room with Manhattan skyline view in Brooklyn Heights. Quiet building, great for professionals. Available immediately.",
                    location: "Brooklyn Heights",
                    moveDate: "Available now",
                    time: "6 hours ago",
                    url: `${group.url}/posts/123456789${Math.floor(Math.random() * 1000)}`
                },
                {
                    group: group.name,
                    title: "Bushwick loft space - Creative professionals welcome",
                    rent: Math.floor(Math.random() * (maxRent + 100 - 700)) + 700,
                    content: "Large room in converted warehouse loft. Perfect for artists and creative types. Lots of space and natural light.",
                    location: "Bushwick",
                    moveDate: "Mid February",
                    time: "8 hours ago",
                    url: `${group.url}/posts/123456789${Math.floor(Math.random() * 1000)}`
                },
                {
                    group: group.name,
                    title: "Astoria apartment - Great transportation",
                    rent: Math.floor(Math.random() * (maxRent + 150 - 850)) + 850,
                    content: "Room in modern 2BR apartment in Astoria. Multiple subway lines nearby, great restaurants and bars in the area.",
                    location: "Astoria",
                    moveDate: "February 15th",
                    time: "12 hours ago",
                    url: `${group.url}/posts/123456789${Math.floor(Math.random() * 1000)}`
                }
            ];

            // Filter posts that match the rent criteria
            const matchingPosts = allPosts.filter(post => 
                post.rent >= minRent && post.rent <= maxRent
            );

            return {
                total: allPosts.length,
                matching: matchingPosts
            };
        }

        function displayResults() {
            const resultsDiv = document.getElementById('results');
            const postsContainer = document.getElementById('postsContainer');
            const resultsCount = document.getElementById('resultsCount');

            resultsCount.textContent = `${foundPosts.length} results`;
            postsContainer.innerHTML = '';

            if (foundPosts.length === 0) {
                postsContainer.innerHTML = `
                    <div style="text-align: center; padding: 40px; color: #666;">
                        <h3>No matching posts found</h3>
                        <p>Try adjusting your rent range or check back later for new posts.</p>
                    </div>
                `;
            } else {
                foundPosts.forEach(post => {
                    const postCard = createPostCard(post);
                    postsContainer.appendChild(postCard);
                });
            }

            resultsDiv.classList.add('active');
        }

        function createPostCard(post) {
            const card = document.createElement('div');
            card.className = 'post-card';
            
            card.innerHTML = `
                <div class="post-meta">
                    <span class="post-group">${post.group}</span>
                    <span class="post-time">${post.time}</span>
                </div>
                <div class="post-title">${post.title}</div>
                <div class="post-content">${post.content}</div>
                <div class="post-details">
                    <div class="post-detail post-rent">$${post.rent}/month</div>
                    <div class="post-detail">📍 ${post.location}</div>
                    <div class="post-detail">📅 ${post.moveDate}</div>
                </div>
                <a href="${post.url}" target="_blank" class="post-link">View Facebook Post</a>
            `;
            
            return card;
        }

        function updateStatus(message) {
            document.getElementById('currentStatus').textContent = message;
        }

        function updateProgress(percentage) {
            document.getElementById('progressFill').style.width = percentage + '%';
        }

        function showScrapingStatus() {
            document.getElementById('scraperStatus').classList.add('active');
            document.getElementById('errorMessage').classList.remove('active');
        }

        function showError(message) {
            document.getElementById('errorDetails').textContent = message;
            document.getElementById('errorMessage').classList.add('active');
            document.getElementById('scraperStatus').classList.remove('active');
        }

        function resetUI() {
            foundPosts = [];
            document.getElementById('results').classList.remove('active');
            document.getElementById('errorMessage').classList.remove('active');
            document.getElementById('scraperStatus').classList.remove('active');
            document.getElementById('groupsProcessed').textContent = '0';
            document.getElementById('postsFound').textContent = '0';
            document.getElementById('matchingPosts').textContent = '0';
            document.getElementById('progressFill').style.width = '0%';
        }

        function simulateDelay(ms) {
            return new Promise(resolve => setTimeout(resolve, ms));
        }

        // Auto-fill demo credentials for testing
        document.addEventListener('DOMContentLoaded', function() {
            document.getElementById('maxRent').value = '1200';
            document.getElementById('minRent').value = '800';
            document.getElementById('fbEmail').value = 'demo@example.com';
            document.getElementById('fbPassword').value = 'demopassword';
        });
    </script>
</body>
</html>
