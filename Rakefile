task :build do
  `haml --style ugly index.haml index.html`
end

task publish: :build do
  `mv index.html /tmp/ && git checkout gh-pages && mv /tmp/index.html . && git add -u && git commit -m publish && git push --all`
end
