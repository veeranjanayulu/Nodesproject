
                            git config user.email "hemanthkumarchintada123@gmail.com"
                            git config user.name "veeranjanayulu"
                            sed -i "s#image:.*#image: ${REPOSITORY_URI}/${AWS_ECR_REPO_NAME}:${BUILD_NUMBER}#g" backend-service.yml
                            git add -A
                            git commit -m "Update deployment image to version ${BUILD_NUMBER}"
                            git push https://${git_token}@github.com/${GIT_USER_NAME}/${GIT_REPO_NAME} HEAD:main
                        