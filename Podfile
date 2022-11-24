platform :ios, '12.0'
use_frameworks!
inhibit_all_warnings!

target 'Parkplus' do
  
  # Pods for Parkplus
  pod 'SwiftGen'
  pod 'Alamofire','~> 4.9.1'
  pod 'GooglePlaces', '4.2.0'
  pod 'GoogleMaps', '4.2.0'
  pod 'TrueSDK'
  pod 'MBProgressHUD'
  pod 'Firebase/Core'
  pod 'Firebase/Crashlytics'
  pod 'Firebase/Analytics'
  pod 'MoEngage-iOS-SDK','~> 7.0'
  pod 'Cosmos'
  pod 'lottie-ios'
  pod 'DeviceKit'
  pod 'Branch'
  pod "CenteredCollectionView"
  pod 'SDWebImage'
  pod 'SDWebImageWebPCoder'
  pod 'SDWebImagePDFCoder'
  pod 'MoEngageInApp','~> 2.0.0'
  pod 'ScrollingPageControl'
  pod 'CTSlidingUpPanel'
  pod 'AppsFlyerFramework'
  pod 'AMPopTip'
  pod 'HyperSDK', '2.0.89'
  pod 'youtube-ios-player-helper'
  pod 'NewRelicAgent'
  pod 'Firebase/RemoteConfig'
  pod 'ReachabilitySwift'
  pod "Connectivity", "~> 5.0"
  pod 'netfox'
  
  target 'ParkplusTests' do
    inherit! :search_paths
    # Pods for testing
  end

  target 'ParkplusUITests' do
    # Pods for testing
  end

end

target 'ParkPlus Notification' do
   pod 'MORichNotification','~>5.0.0'
end
  
post_install do |installer|
 fuse_path = "./Pods/HyperSDK/Fuse.rb"
 clean_assets = false # Pass true to re-download all the assets
 if File.exist?(fuse_path)
   if system("ruby", fuse_path.to_s, clean_assets.to_s)
   end
 end
end
