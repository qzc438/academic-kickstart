---
widget: blank
widget_id: Map
headless: true
weight: 90
title: Map
active: true
design:
  columns: "2"
  background:
    text_color_light: false
    image_darken: 0
---
<body>
    <div id="map-container">
      <div id="locations-panel">
        <div id="locations-panel-list">
          <header>
            <h1 class="search-title">
              <img src="https://fonts.gstatic.com/s/i/googlematerialicons/place/v15/24px.svg"/>
              Find a location near you
            </h1>
            <div class="search-input">
              <input id="location-search-input" placeholder="Enter your address or zip code">
              <div id="search-overlay-search" class="search-input-overlay search">
                <button id="location-search-button">
                  <img class="icon" src="https://fonts.gstatic.com/s/i/googlematerialicons/search/v11/24px.svg" alt="Search"/>
                </button>
              </div>
            </div>
          </header>
          <div class="section-name" id="location-results-section-name">
            All locations
          </div>
          <div class="results">
            <ul id="location-results-list"></ul>
          </div>
        </div>
        <div id="locations-panel-details"></div>
      </div>
      <div id="map"></div>
    </div>
    <script src="https://maps.googleapis.com/maps/api/js?key=AIzaSyBD0nVLmY83UXH372B3nJBScWhQIFIzE-4&callback=initMap&libraries=places,geometry&channel=GMPSB_locatorplus_v4_cABCDE" async defer></script>
  </body>