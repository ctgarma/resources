# resources

https://egghead.io/community/resources


# extensions

ES7 React/Redux/GraphQL/React-Native snippets
dsznajder.es7-react-js-snippets
dsznajder


# Docker for Jenkins

install docker for desktop

docker pull jenkins/jenkins:lts

docker run --detach --publish 8080:8080 --volume
jenkins_home:/var/jenkins_home --name jenkins jenkins/jenkins:lts

docker exec jenkins cat /var/jenkins_home/secrets/initialAdminPassword


# Converting a callback to a Promise

const getDataPromise = (file) => {
  return new Promise ((resolve, reject) => {    
    someUtily.getDataCallback(file, options, (err, data) => {
      if (err) return reject(err)
      resolve(data)
    });
  });
};

# Resources on PM2

https://pm2.keymetrics.io/docs/usage/quick-start/

