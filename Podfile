# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'problem' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!

  # Pods for problem
  pod 'Firebase'
  pod 'Firebase/Auth'
  pod 'Firebase/Analytics'
  pod 'Firebase/Database'
  pod 'Firebase/Storage'
  pod 'Polyline', '~> 4.0'
  pod 'Mapbox-iOS-SDK', '~> 5.9'
  pod 'Firebase/Firestore'
  pod 'FirebaseFirestoreSwift'
  pod 'OAuthSwift'
end

post_install do |installer|
  installer.pods_project.build_configurations.each do |config|
    config.build_settings["EXCLUDED_ARCHS[sdk=iphonesimulator*]"] = "arm64"
  end
end
