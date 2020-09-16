    
    https://developers.google.com/android/reference/com/google/android/gms/ads/identifier/AdvertisingIdClient
    
    try {
            /**
             *   This method cannot be called in the main thread as it may block leading to ANRs. 
             *   An IllegalStateException will be thrown if this is called on themain thread.
             */    AdvertisingIdClient.Info advertisingIdInfo = AdvertisingIdClient.getAdvertisingIdInfo(this);
    
                FLog.d("::::::" +    advertisingIdInfo.getId());
                
            } catch (IOException e) {
                e.printStackTrace();
            } catch (GooglePlayServicesNotAvailableException e) {
                e.printStackTrace();
            } catch (GooglePlayServicesRepairableException e) {
                e.printStackTrace();
            }