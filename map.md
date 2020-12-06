
https://developers.arcgis.com/javascript/
https://developers.arcgis.com/javascript/3/jssamples/exp_history.html
https://github.com/Apress/pro-asp.net-core-mvc/blob/master/Source%20Code%201-31/08%20-%20SportsStore/SportsStore/src/SportsStore/Views/Product/List.cshtml


@model Location
@{
    ViewData["Title"] = "Home Page";
}

<div class="text-center">
    <h1 class="display-4">Map</h1>
    <script>
        function masterfunction() {
            document.getElementById('video_frame').src = "/Map.html?parcelid=1919402007";
            // 1919427020
        }
    </script>
    <button onclick="masterfunction()">Click me</button>

    <iframe src="~/Map.html?parcelid=@Model.ParcelId" height="400" width="600" id="video_frame"></iframe>
</div>

