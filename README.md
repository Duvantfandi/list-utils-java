package com.project;

import com.project.utils.ListUtils;
import java.util.*;

/**
 * Main class to demonstrate the functionality of ListUtils.
 */
public class Main {

    public static void main(String[] args) {

        List<Integer> numbers = Arrays.asList(5, 10, 3, 8, 15, 2, 20);

        // Filter numbers greater than 5 and sort them ascending
        List<Integer> result = ListUtils.filterAndSortList(
                numbers,
                n -> n > 5,
                Integer::compareTo
        );

        System.out.println("Filtered and Sorted List: " + result);
    }
}
