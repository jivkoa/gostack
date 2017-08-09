# gostack

Simple implementation of stack:
https://en.wikipedia.org/wiki/Stack_(abstract_data_type)

## Install

        go get github.com/jivkoa/gostack

## Example

        package main

        import (
                "fmt"
                "github.com/jivkoa/gostack"
        )

        func main() {
                // initialize the slice
                stack := make(gostack.Stack, 0)
                
                // push several elements to the stack
                stack = stack.Push("foo")
                stack = stack.Push("bar")
                
                // pop elements from the stack
                stack, lastEl := stack.Pop() // it returns the slice without the last element and the last elements as well
                
                fmt.Println(lastEl)
        }
