{
 "cells": [
  {
   "cell_type": "code",
   "execution_count": 46,
   "metadata": {},
   "outputs": [],
   "source": [
    "class Test:\n",
    "    @staticmethod\n",
    "    def assert_equals(a, b, *args, **kwargs):\n",
    "        assert a == b\n",
    "        print('Passed')"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "Problem https://edabit.com/challenge/XXJbGFEkrMWCp8yFn (1 point)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 3,
   "metadata": {},
   "outputs": [],
   "source": [
    "def give_me_something(a):\n",
    "    return \"something \" + a"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 4,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Passed\n",
      "Passed\n",
      "Passed\n"
     ]
    }
   ],
   "source": [
    "Test.assert_equals(give_me_something(\"a\"), \"something a\")\n",
    "Test.assert_equals(give_me_something(\"is cooking\"), \"something is cooking\")\n",
    "Test.assert_equals(give_me_something(\" is cooking\"), \"something  is cooking\")"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "Problem https://edabit.com/challenge/TcJXTPJBsfJ2Wgkk4 (2 point)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 10,
   "metadata": {},
   "outputs": [],
   "source": [
    "def paths(n):\n",
    "    if n==1:\n",
    "        return 1\n",
    "    return n *paths(n-1)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 11,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Passed\n",
      "Passed\n",
      "Passed\n",
      "Passed\n",
      "Passed\n",
      "Passed\n",
      "Passed\n",
      "Passed\n"
