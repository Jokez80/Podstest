# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'Podstest' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!

  # Pods for Podstest

  pod 'SwiftSoup'
  pod 'Kingfisher'
  pod 'MBProgressHUD'
  pod 'SQLite.swift'
  pod 'GCDWebServer', podspec: 'https://raw.githubusercontent.com/edrlab/GCDWebServer/3.6.3/GCDWebServer.podspec'
  pod 'R2Shared', podspec: 'https://raw.githubusercontent.com/readium/r2-shared-swift/2.0.0-beta.1/R2Shared.podspec'
  pod 'R2Streamer', podspec: 'https://raw.githubusercontent.com/readium/r2-streamer-swift/2.0.0-beta.1/R2Streamer.podspec'
  pod 'R2Navigator', podspec: 'https://raw.githubusercontent.com/readium/r2-navigator-swift/2.0.0-beta.1/R2Navigator.podspec'
  pod 'ReadiumOPDS', podspec: 'https://raw.githubusercontent.com/readium/r2-opds-swift/2.0.0-beta.1/ReadiumOPDS.podspec'
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
        config.build_settings['SWIFT_VERSION'] = '5.1.4'
        config.build_settings['ENABLE_BITCODE'] = 'NO'
    end
  end
end
