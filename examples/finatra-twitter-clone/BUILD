maven_layout()

target(name='finatra-twitter-clone',
  dependencies=[
    'finatra/examples/finatra-twitter-clone/src/main/scala'
  ]
)

target(name='tests',
  dependencies=[
    'finatra/examples/finatra-twitter-clone/src/test/scala'
  ]
)

jvm_binary(
  name='bin',
  basename='finatra-twitter-clone',
  main='finatra.quickstart.TwitterCloneServer',
  dependencies=[
    ':finatra-twitter-clone'
  ],
  excludes=[
    exclude('org.slf4j', 'slf4j-jdk14'),
    exclude('log4j', 'log4j')
  ]
)
