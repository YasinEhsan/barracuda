## Barracuda
- **Feature** Physical Barriers with notifications

- **Stack** MapKit, CoreLocation, User Notification

- **Takeaway**

| Quick Description  |  How? |  
|---|---|---|
| First commit Xcode remote | git commit -a -m "Commit title here" terminal  |   
|   |   |    
|   |   |    

```Swift
//ONE STOP SHOP BLUE DOT REALTIME

func setupLocationManager(){
    locationManager.delegate = self
    locationManager.desiredAccuracy = kCLLocationAccuracyBest
    locationManager.requestAlwaysAuthorization()
//        locationManager.startUpdatingLocation()  for iphone?
    locationManager.distanceFilter = 100
    mapView.showsUserLocation = true //checkout under shield
}

func centerUserLocation(){
    if let location = locationManager.location?.coordinate {
        let region = MKCoordinateRegion.init(center: location, latitudinalMeters: 10000, longitudinalMeters: 10000)
        mapView.setRegion(region, animated: true)
    }
}

```


<!--![Walkthrough]()-->
<!--![Walkthrough]()-->
<!-- [Visit Project]() -->
