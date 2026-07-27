# Setze hier deine tatsächliche Mindest-iOS-Version (z. B. 13.0 oder 15.0)
platform :ios, '13.0'

target 'Flash Chat iOS13' do
  use_frameworks!

  # Pods for Flash Chat iOS13
  pod 'CLTypingLabel', '~> 0.4.0'

end

# post_install am Ende außerhalb des targets
post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '13.0'
    end
  end
end
