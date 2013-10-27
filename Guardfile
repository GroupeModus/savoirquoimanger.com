guard 'shell' do
  #watch(/(^src\/haml\/(.+)\.haml)/) do |match|
    #puts match[0] + " changed at " + Time.now.strftime("%H:%M:%S") +". Re-generating HTML from HAML"
    #`haml #{match[1]} #{match[2]}.html`
    #`terminal-notifier -group 'haml' -title 'Regenerating Coffeescript' -message '#{match[0]}'`
  #end

  watch(/(^src\/sass\/.+)/) do |match|
    puts match[0] + " changed at " + Time.now.strftime("%H:%M:%S") +". Re-generating CSS from SASS."
    `Compass compile`
    `terminal-notifier -group 'compass' -title 'Regenerating Compass' -message '#{match[0]}'`
  end

  #watch(/(^src\/coffeescript\/.+)/) do |match|
    #puts match[0] + " changed at " + Time.now.strftime("%H:%M:%S") +". Re-generating JS from CoffeeScript"
    #`coffee -c -o assets/javascripts src/coffeescript`
    #`terminal-notifier -group 'coffeescript' -title 'Regenerating Coffeescript' -message '#{match[0]}'`
  #end
end
