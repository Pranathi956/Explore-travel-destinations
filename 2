<!DOCTYPE html>
<html>
<head>
	<title>Explore travel destinations</title>
	<style>
	<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css"> 
	body{
			background-image:url('img2.jpeg');
			background-size:cover;
		}
	.btn{
		text-decoration:none;
		width:250px;
		margin-top:10px;
		border:none;
		background-color:transparent;
		font-size:14px;
		color:black;
	}
	.bottom{
		position: relative;
		bottom: 0;
		border-top:2px solid blue;
		width:100%;
		margin:0px;
		padding:5px;
		text-align:center;
		background-color:#FAF0BE;
	}
	*{
		margin:0px;
		padding:0px;
	}
	
	.filter{
		width:100%;
		padding:5px;
		text-align:center;
		background-color:#1F456E;
	}
	.filter button, .favorite-btn, .display-btn ,.book-btn,.remove-btn, .show-favs-btn {
            padding: 10px 15px;
            margin: 5px;
			margin-top:10px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
            background: #daf0ff;
            color: black;
        }
        .show-favs-btn {
            background: #1F456E;
        }
        .destinations, .favorites {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }
        .destination, .favorite-item,.favorites-container {
			color:white;
            background: #1F456E;
            width: 250px;
			height:150px;
			justify-content: center;
            margin: 15px;
            padding: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            cursor: pointer;
            border-radius: 10px;
            transition: transform 0.2s ease;
        }
        .destination:hover {
            transform: scale(1.05);
        }
        .modal {
			color:pink;
            display: none;
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background: #1F456E;
            padding: 20px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.3);
            width: 300px;
			height:130px;
			border-radius:5px;
			justify-content:center;
            border-radius: 10px;
        }
        .modal h2 {
            margin-bottom: 10px;
        }
        .close {
            background:#daf0ff;
            color: black;
            padding: 5px 10px;
            cursor: pointer;
            border: none;
            margin-top: 10px;
        }
        #favorites-container {
            display: none; 
        }
	</style>
</head>
<body>
	<center>
	
	<div class="filter">
        <button onclick="filterDestinations('all')">All</button>
        <button onclick="filterDestinations('beach')">Beaches 🏖️</button>
        <button onclick="filterDestinations('mountain')">Mountains 🌄</button>
        <button onclick="filterDestinations('city')">Cities 🏙️</button>
        <button class="show-favs-btn" onclick="toggleFavorites()">Show Favorites ⭐</button>
    </div><hr style="border-bottom:4px solid black;">
	

    <div class="destinations" id="destinations"></div>

    <div id="favorites-container">
        <h2 style="background-color:#1F456E; margin-bottom:20px; color:white;">Your Favorites ❤️</h2>
        <div class="favorites" id="favorites"></div>
    </div>

    <div id="modal" class="modal">
        <h2 id="modal-title"></h2>
        <p id="modal-description"></p>
        <p><strong>Best Time to Visit:</strong> <span id="modal-time"></span></p>
        <button class="close" onclick="closeModal()">Close</button>
    </div>
	</center>
    <script>
        const destinations = [
            { name: "Bali, Indonesia 📍", category: "beach", description: "Stunning beaches and culture.", bestTime: "April - October" },
            { name: "Maldives 📍", category: "beach", description: "Crystal clear waters & luxury resorts.", bestTime: "November - April" },
            { name: "Santorini, Greece 📍", category: "beach",  description: "White-washed buildings & blue waters.", bestTime: "May - September" },
			{ name: "Bora Bora, French Polynesia 📍", category: "beach", description: "Overwater bungalows & turquoise lagoons.", bestTime: "May - October" },
			{ name: "Maui, Hawaii, USA 📍", category: "beach", description: "Golden beaches & volcanic landscapes.", bestTime: "April - October" },
			{ name: "Phuket, Thailand 📍", category: "beach", description: "Lively nightlife & stunning beaches.", bestTime: "November - April" },
			{ name: "Seychelles 📍", category: "beach", description: "Unspoiled beaches & exotic marine life.", bestTime: "April - October" },
			{ name: "Andes, Peru 📍", category: "mountain", description: "Home to Machu Picchu & breathtaking trails.", bestTime: "May - September" },
			{ name: "Dolomites, Italy📍", category: "mountain", description: "Dramatic peaks & alpine villages.", bestTime: "June - September" },
			{ name: "Banff National Park, Canada 📍", category: "mountain", description: "Lakes, wildlife & snowy peaks.", bestTime: "June - September" },
			{ name: "Patagonia, Argentina & Chile 📍", category: "mountain", description: "Glaciers, rugged landscapes & adventure.", bestTime: "October - March" },
            { name: "Swiss Alps, Switzerland📍", category: "mountain", description: "Perfect for skiing and scenic views.", bestTime: "December - April" },
            { name: "Mount Everest, Nepal 📍", category: "mountain",description: "Highest peak in the world!", bestTime: "April - June" },
            { name: "Rocky Mountains, Canada 📍", category: "mountain", description: "Breathtaking nature & hiking trails.", bestTime: "June - September" },
			{ name: "Barcelona, Spain 📍", category: "city", description: "Vibrant nightlife & Gaudi architecture.", bestTime: "April - June" },
			{ name: "Istanbul, Turkey 📍", category: "city", description: "East meets West with rich history.", bestTime: "April - June, September - October" },
			{ name: "Seoul, South Korea📍", category: "city", description: "Tech hub with a mix of tradition.", bestTime: "April - May, September - October" },
			{ name: "Rome, Italy 📍", category: "city", description: "Ancient ruins & world-famous cuisine.", bestTime: "April - June, September - October" },
            { name: "Tokyo, Japan 📍", category: "city", description: "Modern city with a rich culture.", bestTime: "March - May" },
            { name: "New York, USA 📍", category: "city", description: "The city that never sleeps.", bestTime: "April - June" },
            { name: "Paris, France 📍", category: "city", description: "Romantic city with iconic landmarks.", bestTime: "April - October" },
            { name: "Dubai, UAE 📍", category: "city",  description: "Luxury, skyscrapers & desert adventures.", bestTime: "November - March" },
			{ name: "Singapore 📍", category: "city", description: "Futuristic skyline & cultural diversity.", bestTime: "February - April" },
			{ name: "London, UK 📍", category: "city", description: "Historic landmarks & vibrant culture.", bestTime: "May - September" }

        ];

        let favorites = [];

        function displayDestinations(filteredCategory = 'all') {
            const container = document.getElementById("destinations");
            container.innerHTML = "";

            destinations
                .filter(dest => filteredCategory === 'all' || dest.category === filteredCategory)
                .forEach(dest => {
                    const div = document.createElement("div");
                    div.classList.add("destination");
                    div.innerHTML = `
                        <h3>${dest.name}</h3>
                        <button class="favorite-btn" onclick="addToFavorites(event, '${dest.name}')">⭐ Add to Favorites</button>
						 <button class="display-btn" onclick="openModal(event, '${dest.name}')">📜 Details</button> 
						 <button class="book-btn" onclick="bookTicket(event, '${dest.name}')">🎟️ Book Ticket</button>
                    `;
                    div.onclick = (event) => {
                        if (!event.target.classList.contains('favorite-btn')) {
                            openModal(dest);
                        }
                    };
                    container.appendChild(div);
                });
        }

        function filterDestinations(category) {
            displayDestinations(category);
        }

        function addToFavorites(event, name) {
            event.stopPropagation(); 
            if (!favorites.includes(name)) {
                favorites.push(name);
                displayFavorites();
            }
        }

        function removeFromFavorites(name) {
            favorites = favorites.filter(fav => fav !== name);
            displayFavorites();
        }

        function displayFavorites() {
            const favContainer = document.getElementById("favorites");
            favContainer.innerHTML = "";

            if (favorites.length === 0) {
                document.getElementById("favorites-container").style.display = "none";
                return;
            }

            document.getElementById("favorites-container").style.display = "block";

            favorites.forEach(name => {
                const div = document.createElement("div");
                div.classList.add("favorite-item");
                div.innerHTML = `
                    <h3>${name}</h3>
                    <button class="remove-btn" onclick="removeFromFavorites('${name}')">❌ Remove</button>
                `;
                favContainer.appendChild(div);
            });
        }

        function toggleFavorites() {
            const favSection = document.getElementById("favorites-container");
            favSection.style.display = favSection.style.display === "none" ? "block" : "none";
        }
		function bookTicket(event, name) {
            event.stopPropagation();
            alert(`🎉 Your ticket to ${name} has been booked!`);
        }

        
		function openModal(event, name) {  
            event.stopPropagation();
            const dest = destinations.find(d => d.name === name);
            document.getElementById("modal-title").innerText = dest.name;
            document.getElementById("modal-description").innerText = dest.description;
            document.getElementById("modal-time").innerText = dest.bestTime;
            document.getElementById("modal").style.display = "block";
        }

        function closeModal() {  
            document.getElementById("modal").style.display = "none";
        }

        displayDestinations();
    </script>
	<div class="bottom">
		<button class="btn">Support centre</button>
	</div>
</body>
</html>
