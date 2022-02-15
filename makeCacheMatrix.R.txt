makeCacheMatrix <- function(a = matrix()) {
  k <- NULL
  set <- function(b){
  a <<- b
  k <<- NULL
  }
  get <- function()a
  setInverse <- function(inverse) k <<- inverse
  getInverse <- function() j 
  list(set = set, get = get, 
  setInverse = setInverse, 
  getInverse = getInverse)
}